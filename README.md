# Custom Map Loader - Rooftops & Alleys
### Mod Version: Public Beta 1 - At the moment, this mod is being re-made to fit in the main menu. This mod also loads map directly from their name. A list with your installed maps will be added as soon as possible. For help or question, add me on Discord: [LoulouNoLegend](https://discord.com/users/421740856303812630)
If you are only a player, read the player section. If you are a mapper, read the two sections so your map can work correctly!

Feel free to join the Discord Server by [clicking here](https://discord.gg/kHZVQyVWFq)

## A) For Players and Modders
To open a map, follow the section **B-5**. It works the same way.

If the mod is correctly installed, it should normally open the map loader menu. For now, the map loader works by entering the name of the custom map. In the future, a list should be added to directly select it.

![image](https://github.com/LoulouNoLegend/CustomMapLoader-RooftopsAndAlleys/assets/40952934/8d1561e5-7232-4de0-a9e0-859778b1b254)


After entering the map name, click on Load and enjoy!

If the map name is not working, be sure that it's writted correctly or try the other method. Enjoy!


## B) Only for Modders
Right now, there's a lot of possible errors when cooking a map and it still unclear why we get them.


### B-1) What you need installed to make a custom map
- Epic Games Launcher
  - Unreal Engine 5.2.1
- Rooftops & Alleys.. to test the mod.

### B-2) How to setup the project
**1.** Download the template project by clicking [here](https://github.com/LoulouNoLegend/CustomMapLoader-RooftopsAndAlleys/releases/download/PB1/CustomMapLoader_Template.zip)
**2.** Extract the "rooftopsandalleys" folder somewhere on your pc.
**3.** Open the folder and then the "rooftopsandalleys.uproject" file.
**4.** In your content folder, rename the file `Label_MapName` to your liking by keeping the `Label_` at the start of the name. *(Right click on the file to rename or press F2)*

![image](https://github.com/LoulouNoLegend/CustomMapLoader-RooftopsAndAlleys/assets/40952934/2f96f4af-95df-4039-b3d2-35fccd7dae3d)


**5.** Open the file you renamed. The only setting you need to change is the second one. Change the *Chunk ID* to a number between 1 and 100 000, then close the file.

![image](https://github.com/LoulouNoLegend/CustomMapLoader-RooftopsAndAlleys/assets/40952934/f42e4923-a3ca-4c14-9ae8-cf5c6f817a52)

**6.** After that, just go inside the *CustomMaps* folder, right click and create a folder for all of your assets that has the name of your map *(not an obligation, but the name need to be unique to not interfer if the user as multiple custom maps installed)*

**7.** Create your map! If you need help to understand how Unreal Engine works to create maps, there's good tutorials on YouTube.

### B-3) Package your project
**1.** Go to *Platforms > Windows* and click on *Package Project*.
**2.** A window with the folders of your PC should appear in the screen. Create a folder somewhere on your PC, select it and click on *Select the folder* or *Open* at the bottom right of the file explorer.
**3.** It should now be starting to package.

![image](https://github.com/LoulouNoLegend/CustomMapLoader-RooftopsAndAlleys/assets/40952934/4e104f25-faaa-4faa-a9f8-08bc33a46c02)

### B-4) Install your map into the game
**1.** Go to where you decided to package your map.
**2.** Go into *Windows > rooftopsandalleys > Content > Paks*.
**3.** There should be some files. The important ones are the ones with the *chunk number* you set earlier in the *Asset Data* file.

![image](https://github.com/LoulouNoLegend/CustomMapLoader-RooftopsAndAlleys/assets/40952934/5dac8e6a-6f82-430a-a119-fe0a2a6517b0)

**4.** Select all these files and rename them to the name of your level, adding `_P` at the end. It should look like this.

![image](https://github.com/LoulouNoLegend/CustomMapLoader-RooftopsAndAlleys/assets/40952934/fa120c38-47bf-43e0-98ac-07ba2f6671fd)

**5.** Don't close the file explorer, we will need to copy these 3 files somewhere. Find and go into the files of your *Rooftops & Alleys* game. You can simply go in steam, right click on your game and go to *Manage > Browse local files*.

![image](https://github.com/LoulouNoLegend/CustomMapLoader-RooftopsAndAlleys/assets/40952934/b146280b-efc2-47cc-9f24-8730a2c79162)

**6.** It should open a file explorer right into the files of the game. Go to *RooftopsandAlleys > Content > Paks* and create a folder named *mods*.

![image](https://github.com/LoulouNoLegend/CustomMapLoader-RooftopsAndAlleys/assets/40952934/f07bc7b5-5d6d-4b49-8a54-3e6afc76c060)

**7.** Go into the *mods* folder and copy the 3 files in there.

### B-5) Launch your map with Custom Map Loader
**1.** Launch the game. When in the menu, go to *Tutorials > Advanced*. The CML menu should load. Enter the name of your level into the text box and click Load.

![image](https://github.com/LoulouNoLegend/CustomMapLoader-RooftopsAndAlleys/assets/40952934/cfcc5947-0222-4d86-b8d4-ad971c5b9981)

**2.** If it doesn't work, first make sure your correctly entered the name of the level. If it was the case and it still doesn't load, try the second text box.

![image](https://github.com/LoulouNoLegend/CustomMapLoader-RooftopsAndAlleys/assets/40952934/074b4b42-b331-4fe9-95d3-4c71cad11b42)

**3.** If it still doesn't work, be sure that your correctly set up your *chunk number* or that the map cooked correctly. If you really need more help, join the [Rooftops And Alleys Discord Server](https://discord.gg/kHZVQyVWFq).

If it works, enjoy and share it with others!

## C) FAQ

### C-1) Why `CM_`?
It is simply a way to easily recognize mods that are a custom map.

### C-2) Is it possible to release a mod with multiple custom maps in it?
It totally is possible, just try to follow the recommended file structure with each map having it's level in `Content/CustomMaps` and their own folder containing all their assets.
