## botanic gardens
curl 192.168.33.10:8002/isochrone --data '{"locations": [{"lat": 1.3155535, "lon": 103.8133094}], "costing": "auto", "contours": [{"time": 1}, {"time": 2}, {"time": 3}, {"time": 4}, {"time": 5}, {"time": 6}, {"time": 7}, {"time": 8}, {"time": 9}, {"time": 10}, {"time": 11}, {"time": 12}, {"time": 13}, {"time": 14}, {"time": 15}, {"time": 16}, {"time": 17}, {"time": 18}, {"time": 19}, {"time": 20}, {"time": 21}, {"time": 22}, {"time": 23}, {"time": 24}, {"time": 25}, {"time": 26}, {"time": 27}, {"time": 28}, {"time": 29}, {"time": 30}], "polygons": true, "denoise": 0.2, "generalize": 100}' > test.json

## gedong camp
curl 192.168.33.10:8002/isochrone --data '{"locations": [{"lat": 1.4174517, "lon": 103.6990203}], "costing": "auto", "contours": [{"time": 1}, {"time": 2}, {"time": 3}, {"time": 4}, {"time": 5}, {"time": 6}, {"time": 7}, {"time": 8}, {"time": 9}, {"time": 10}, {"time": 11}, {"time": 12}, {"time": 13}, {"time": 14}, {"time": 15}, {"time": 16}, {"time": 17}, {"time": 18}, {"time": 19}, {"time": 20}, {"time": 21}, {"time": 22}, {"time": 23}, {"time": 24}, {"time": 25}, {"time": 26}, {"time": 27}, {"time": 28}, {"time": 29}, {"time": 30}], "polygons": true, "denoise": 0.2, "generalize": 100}' > test.json

## flora drive
curl 192.168.33.10:8002/isochrone --data '{"locations": [{"lat": 1.3565307, "lon": 103.9631898}], "costing": "auto", "contours": [{"time": 2}, {"time": 4}, {"time": 6}, {"time": 8}, {"time": 10}, {"time": 12}, {"time": 14}, {"time": 16}, {"time": 18}, {"time": 20}, {"time": 22}, {"time": 24}, {"time": 26}, {"time": 28}, {"time": 30}], "polygons": true, "denoise": 0.2, "generalize": 100}' > test.json

# botanic gardens 2/4/6/8
curl 192.168.33.10:8002/isochrone --data '{"locations": [{"lat": 1.3155535, "lon": 103.8133094}], "costing": "auto", "contours": [{"time": 2}, {"time": 4}, {"time": 6}, {"time": 8}, {"time": 10}, {"time": 12}, {"time": 14}, {"time": 16}, {"time": 18}, {"time": 20}, {"time": 22}, {"time": 24}, {"time": 26}, {"time": 28}, {"time": 30}], "polygons": true, "denoise": 0.2, "generalize": 100}' > test.json

# KLCC 2/4/6/8
curl 192.168.33.10:8002/isochrone --data '{"locations": [{"lat": 3.1468059, "lon": 101.6897892}], "costing": "auto", "contours": [{"time": 2}, {"time": 4}, {"time": 6}, {"time": 8}, {"time": 10}, {"time": 12}, {"time": 14}, {"time": 16}, {"time": 18}, {"time": 20}, {"time": 22}, {"time": 24}, {"time": 26}, {"time": 28}, {"time": 30}], "polygons": true, "denoise": 0.2, "generalize": 100}' > test.json
