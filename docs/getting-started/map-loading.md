# Map Loading

This section of the d.ASH SDK documentation provides details about file organisation of autonomy maps for the d.ASH SDK. 

To load a new map, upload the autonomy map files in the folder `maps` found in `/dash_sdk/.data/maps`. Please ensure that the following files are in the folder:

```
dash-sdk/
└─ .data/
    └─ maps
        └─ <MAP_NAME>.png       # 2D Autonomy Map
        └─ <MAP_NAME>.pcd       # 3D Autonomy Map
        └─ <MAP_NAME>.json      # Global Planner Configuration
```


To activate the new map, ensure the map name in [`auto_config.json`](\dash-sdk\sdk-config\auto-config) file matches `<MAP_NAME>`. For example: 

```
"map_name": "outdoor_map",
```