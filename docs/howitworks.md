
### Partitioning

You will have to install Skyrim, in Steam, on a different drive than the default drive C: for reasons explained further below. This means that you need to have more than one partition (or hard drive).

Therefore, if your PC and portable device have only a drive C:, use a partitioning tool and create a new partition with a few hundred MBs of space for the entire Skyrim installation, and mount it as drive D: (or E: or whatever you prefer).

### Windows only

This entire setup currently focuses on Windows only. While it can most likely also be achieved on Linux systems, possibly even on a mixed setup (e.g. Windows gaming PC and Linux Steam Deck), that makes things even more complicated, so it's a topic for another day. To keeps things as streamlined as possible, this article focuses on a Windows-only setup.

### ModOrganizer 2

For modding Skryim, the tool "ModOrganizer 2", or "MO2" in short, will be used. It may be possible to do all this with other modding tools too, but that's outside the scope of this documentation.

This example also assumes that there is a drive D: where everything will be installed. The final directory layout would look something like this:

```bash
\Skyrim Modding\         - directory for modding-related tools and modding data
\Skyrim Special Edition\ - user settings and game saves
\SteamLibrary\           - the directory where Steam installs the game.
```

Note that the directory "Skyrim Special Edition" will actually need to be soft-linked to a location in the user's home directory. This is because Skyrim by default uses a path in the users home directory ("$HOME\Documents\My Games\Skyrim Special Edition") to store the saves. 

But since the usernames may be different between the two computers, we want to externalize this data onto the same drive where the game itself is, and will use a soft-link for that. Of course we could attempt to sync the saves between the two home directories directly, but permission issues may arise and prevent that (as the user running a sync from the PC may not have permission to write into the home directory of the user on the other system). This whole linking setup is explained in detail further below. 


