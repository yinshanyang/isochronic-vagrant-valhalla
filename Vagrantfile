Vagrant.configure(2) do |config|
  config.vm.provider "virtualbox" do |v|
    v.name = "sandbox-isochrone"
    v.memory = 5120
    v.cpus = 2
  end

  config.vm.box = "envimation/ubuntu-xenial-docker"
  config.vm.network "private_network", ip: "192.168.33.10"

  config.vm.provision "shell", inline: <<-SHELL
    # install dependencies and valhalla
    sudo apt-get update
    sudo apt-get install --yes software-properties-common python
    sudo add-apt-repository --yes ppa:valhalla-core/valhalla
    sudo apt-get update
    sudo apt-get install --yes valhalla-bin

    # download osm.pbf
    mkdir data
    curl https://download.bbbike.org/osm/bbbike/Singapore/Singapore.osm.pbf > data/singapore.osm.pbf

    # prepare valhalla
    mkdir valhalla
    valhalla_build_config --mjolnir-tile-dir ${PWD}/valhalla --mjolnir-tile-extract ${PWD}/valhalla.tar --mjolnir-timezone ${PWD}/valhalla/timezones.sqlite --mjolnir-admin ${PWD}/valhalla/admins.sqlite > valhalla.json
    valhalla_build_tiles -c valhalla.json data/singapore.osm.pbf
    # find valhalla | sort -n | tar cf valhalla.tar --no-recursion -T -
  SHELL
end
