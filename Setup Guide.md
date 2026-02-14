# Setup Guide
This requires...
- The APWorld from the [Releases Page](https://github.com/Nichologeam/VRChat-AP/releases)
- The custom build of Udon-MIDI-Web-Helper from the [Releases Page](https://github.com/Nichologeam/VRChat-AP/releases)
- [loopMIDI](https://www.tobias-erichsen.de/software/loopmidi.html) by Tobias Erichsen

1. Generate a Multiworld with the VRChat .yaml
2. Launch the VRChat Client from the Archipelago Launcher and *do not connect*
3. Launch Udon-MIDI-Web-Helper
4. Launch VRChat and create a new instance of the [VRChat Archipelago Client](https://vrchat.com/home/launch?worldId=wrld_9f4b45a2-4209-4d83-ae46-e63449c7575c) world
5. Wait for the VRChat Client to receive the STATUS OK signal from VRChat (will say "Ready to connect to the multiworld!")
6. Connect to the Multiworld!

# Troubleshooting
You must start the Udon-MIDI-Web-Helper.exe *before* you start VRChat. It will not work otherwise. If Udon-MIDI-Web-Helper connects, but the game is not responding to it, restart VRChat with the `--midi=Udon-MIDI-Web-Helper` launch option. Make sure you followed the connection instructions in order. 

Check the VRChat Client for any errors. I've included debug messages for a lot of the server and client communication. If it's nothing obvious, try recreating the issue with the Archipelago Debug Launcher, named ArchipelagoLauncherDebug.exe inside your Archipelago folder.

If the issue is with the VRChat world, I've left World Debugging enabled. Press `Right Shift + ~ + 3` to pull up a logging UI (this may require the `--enable-debug-gui` launch option). Send me a screenshot of the UI, including any errors that may be in it.

Please report bugs if you find them. This is held together with duct tape and a dream.

# Usage
The physics-enabled cubes on the left are your locations. Place them into the bin on the right of the text client to send them.

The floating cubes on the left are the DeathLink testing cubes. The colored one can be used to toggle DeathLink, while the uncolored one sends a DeathLink.

The floating spheres on the right are a rudementary tracker. They will turn green when you receive their respective Puzzle Unlock items.
