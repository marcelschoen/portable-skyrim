### Install "FreeFileSync"

* Download from [FreeFileSync Homepage](https://freefilesync.org/)
* Install wherever you want (not important)
* Prepare the following 3 sync profiles (click the "New" icon):

    * "FullSkyrimSync_PC2portable": 
         * left side: "D:"
         * right side= "X:"
         * sync type: "Synchronise Mirror ->"
         * Will be used initially to sync the entire Skyrim setup from PC to portable

    * "SkyrimModsSync_PC2portable"
         * left side: D:\Skyrim Modding\MO2 Data
         * right side: X:\Skyrim Modding\MO2 Data
         * sync type: "Synchronise Mirror ->"
         * Can be used every time mods are installed or changed on the PC, to sync the mod setup to the portable

    * "SkyrimSyncSaves" 
         * left side: D:\Skyrim Special Edition\Saves
         * right side: X:\Skyrim Special Edition\Saves
         * sync type: "Synchronize Two Way <-->"
         * Allows to sync the game saves in both directions

That's it - you're done. Kind of. In the sense that you now have everything in place to get your modded multi-device game started. 

IMPORTANT HINT: Whenever you run the sync tool, make sure the shared directory is actually mounted in that moment. If you have, for example, your AyaNeo sitting in its dock, it may have switched off after a while, and the drive X: may not respond anymore. Make sure your portable is on, and quickly open the mounted drive X: manuall in the desktop explorer, before running the sync tool.

