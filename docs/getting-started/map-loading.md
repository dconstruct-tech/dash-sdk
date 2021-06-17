# Map Loading

This section of the d.ASH SDK documentation provides details about file organisation of autonomy maps for the d.ASH SDK. 

1. To load a new map, upload the autonomy map files in the following location:
```
/dash_sdk/.data/maps/<MAP_NAME>
```
For example, if your map is `outdoor_map.pcd`,
```
/dash_sdk/.data/maps/outdoor_map
```

2. Within that folder, ensure the following files are in the folder:

    - 2D Autonomy Map: `<MAP_NAME>.png`
    - 3D Autonomy Map: `<MAP_NAME>.pcd`
    - Global Planner Configuration: `<MAP_NAME>.json`



3. To activate the new map, ensure the map name in [`auto_config.json`](/sdk-config/auto-config) file matches `<MAP_NAME>`.
```
"map_name": "outdoor_map",
```