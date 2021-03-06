# Arnold For Blender 2.80 (BtoA) Beta
[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=5D8ZMMACFUX36)

<p align="center">
<img src="https://rawcdn.githack.com/tyler-furby/Arnold-For-Blender/b194477da00ea4ab76d0acf0722be2be51df0075/arnold%20logo.svg" alt="Blender One Logo" width="50%">
</p>

Arnold integration with Blender, updated to work with the latest versions of Arnold and Blender 2.8. This is not yet production ready, but will be soon... :balloon:

Join the Discord channel for discussions/help/updates/feature requests/talk about water coolers: https://discord.gg/M7K8Tw8

Update: Working on the offical version of this addon, will post more information as that project progresses further.

```
Blender One Roadmap                   [####                     ] 20% Complete
```
### Currently In Development: 
- OpenGL / Optix / RTX IPR (rendered viewport)
- Fixing Occasional Particle System Crash
- Adding procedurals
- Streamling with Eevee, Cycles, and Workbench Render Engines
- Adding Math Nodes, and more
- VDB Support
- Launching a custom build which comes packaged with Arnold Render by default.

### Installation (Windows, macOS, and Linux)
- Download this repository.
- Download the latest Arnold SDK here: https://www.solidangle.com/arnold/download/#arnold-sdk
- Add a new environment variable `ARNOLD_HOME` and add the path of the downloaded arnold SDK from the previous step.
- Add a second environment variable to `PATH` to the arnold SDK `bin` folder.
- Add `barnold` directory to `path\to\blender\2.80\scripts\addons`
- If you are on **macOS**:
  - Simply type this into terminal: `launchctl setenv ARNOLD_HOME "/path/to/ArnoldSDK"`
 - If you are on **Linux**
    - Create a file called `arnold.sh` inside `etc/profile.d` and put your `ARNOLD_HOME` environment variable in there. 
- Open the `Arnold SDK Adjustments\plugins` folder the `driver_display_callback.dll` (Windows) or `libbarnold_display_callback.dylib` (macOS) or `libbarnold_display_callback.so` (Linux) file needs to be placed inside the `ARNOLDSDK\plugins` folder.
- Open the `Arnold SDK Adjustments\arnold` folder, the `ai_drivers.py` file needs to be placed inside the `ARNOLDSDK\python\arnold` folder, overwriting the existing file.
- Open the `Arnold SDK Adjustments\arnold` folder, the `ai_universe.py` file needs to be placed inside the `ARNOLDSDK\python\arnold` folder, overwriting the existing file. 
- Enable "Auto Run Python Scripts" in blender by going to File>User Preferences>File tab 
- Enable the plugin in blender by going to File>User Preferences>Add-ons tab>Search for 'arnold' in the search bar, and clicking the checkbox next to `Render: Barnold` to enable this plugin.

### Complete BtoA Documentation (coming soon)

### About
I'm actively working on this every day, if you have any issues feel free to contact me at tyler@tylerfurby.com,
I will ensure this plugin supports all future updates to Blender and Arnold renderer.

![Blender loves arnold](https://cdn.rawgit.com/tyler-furby/Furby-Studios-Website-Files/a449e03a/images/Untitled-1.png)
