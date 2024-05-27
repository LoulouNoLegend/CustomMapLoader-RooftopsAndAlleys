
# Custom Map Loader - Rooftops & Alleys
### Mod Version: Public Beta 1 - At the moment, this mod is being re-made to fit in the main menu. This mod also loads map directly from their name. A list with your installed maps will be added as soon as possible. For help or question, add me on Discord: [LoulouNoLegend](https://discord.com/users/421740856303812630)
If you are only a player, read the player section. If you are a mapper, read the two sections so your map can work correctly!

## For Players and Modders
**Enter the menu:**
In the main menu go to *Tutorials > Advanced*.

If the mod is correctly installed, it should normally open the map loader menu. For now, the map loader works by entering the name of the custom map. In the future, a list should be added to directly select it.

![image](https://github.com/LoulouNoLegend/CustomMapLoader-RooftopsAndAlleys/assets/40952934/8d1561e5-7232-4de0-a9e0-859778b1b254)


After entering the map name, click on Load and enjoy!

If the map name is not working, be sure that it's writted correctly or try the other method. Enjoy!


## Only for Modders

### The project
Firstly, you need to create an empty project in Unreal Engine 5.2.1 named "rooftopsandalleys", the same way as if you were doing a Rooftops & Alleys mod.

After opening the project, create an *Asset Data* object inside the "Content" folder.

To create an *Asset Data*, you can follow this little tutorial by Rpatty: [Click Here](https://cdn.discordapp.com/attachments/1156177948597047398/1243325692029177856/2024-05-23_23-10-28.mp4?ex=66550548&is=6653b3c8&hm=69164740dfb766d639d2ff5943109b66656d480a5de12fb3bb0aaec8c9aa1040&)


When creating your map, here's some tips:
### The folders and how to place your files
All your content need to be places in a specific way to work correctly and not interfer with other custom maps.

Create a *CustomMaps* folder inside the *Content* folder where you can place your level.
If you want, you can add the `CM_` prefix to your map name, to simply specify that your mod is a custom map. (Ex: `CM_DustCS2`)

⚠️ **Be sure to place every assets and sub folders (ex: textures, materials..) of your map in a folder that is the same name as your map to prevent that if the user as multiple custom maps, they don't break each-others!**

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
If your mod is not using `CM_`, just enter the map name and the suffix `_P`.

Share it and you are done!


## FAQ

### Why `CM_`?
It is simply a way to easily recognize mods that are a custom map.

### Is it possible to release a mod with multiple custom maps in it?
It totally is possible, just try to follow the recommended file structure with each map having it's level in `Content/CustomMaps` and their own folder containing all their assets.
