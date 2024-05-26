
# Custom Map Loader - Rooftops & Alleys
### Mod Version: Public Beta 1

If you are only a player, read the player section. If you are a mapper, read the two sections so your map can work correctly!

## For Players
**Enter the menu:**
In the main menu go to *Tutorials > Advanced*.

If the mod is correctly installed, it should normally open the map loader menu. For now, the map loader works by entering the name of the custom map. In the future, a list should be added to directly select it.

![image](https://github.com/LoulouNoLegend/CustomMapLoader-Rooftops-Alleys/assets/40952934/9eaa872d-c364-4822-a2b7-9a01444f07c9)


You don't need to include `CM_` when entering the name of the map in the *Level Name* entry, since the mod already writes it. This prefix is only a way for modders to make their map be recognized correctly by the map loader.

After entering the map name, click on Load and enjoy!

If the map name is not working, be sure that it's writted correctly. Enjoy!



## For Modders / Mappers

When creating your map, here's some tips to follow:
### The folders and how to place your files
All your content need to be places in a specific way to work correctly and not interfer with other custom maps.

Create a *CustomMaps* folder inside the *Content* folder where you can place your level, and named with the `CM_` prefix. (Ex: `CM_DustCS2`)

```
└── Content/
    └── CustomMaps/
        └── CM_YourMap
            CM_YourMap/
            └── Blueprints/
                ...
```

In unreal, it would be like this (From the *CustomMaps* folder):

![Capture d’écran 2024-05-26 124021](https://github.com/LoulouNoLegend/CustomMapLoader-Rooftops-Alleys/assets/40952934/a9e01c1f-6762-49ef-8907-6ef5e931f324)



### The mod itself

When your map is complete and packed, do this:
- Rename the 3 files of your package to the name of your map
- Add `_P` at the end of every files so the game recognize the mod

After all that, your 3 files should look like this: `CM_MapName_P.<fileExtention>`

Share it and you are done!
