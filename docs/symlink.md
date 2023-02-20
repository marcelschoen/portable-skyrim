### Prepare symlink for settings and saves

Now we prepare the soft-link for the directory with the game saves and settings:

- In your home directory, find this subdirectory: "Documents\My Games\Skyrim Special Edition".
- _Move_ the "Skyrim Special Edition" folder entirely to drive D:, so that you end up with "D:\Skyrim Special Edition"
- Now create a soft-link pointing to this directory in the location where it originally was:
- Open a DOS shell and change into the subdirectory by entering

```  
    cd "Documents\My Games"
```

- create the link by running

```
    mklink /D "Skyrim Special Edition" "D:\Skyrim Special Edition"
```

- If you now run a simple "dir" command, you should see a line like this:

```
    17/12/2022  20:53    <SYMLINKD>     Skyrim Special Edition [D:\Skyrim Special Edition]
```

Now whenever Skyrim stores a save game into the folder "$HOME\Documents\My Games\Skyrim Special Edition", it will actually be stored on drive D:, where it can easily be accessed by the syncing tool.
