# Gaming
A place for all my Linux gaming related stuffs
<!--
<hr>
## Game

<b>Steps:</b><br><br>

<br><br>
<b>Steam Arguments:</b> 
```bash
Arguments go here
```
-->
## <h2>Useful Info - Steam</h2>
Move default pfx location on steam<br>

```bash
STEAM_COMPAT_DATA_PATH= %command%
```
<br>
The target path needs to be inside quotations, important to check when changing the path to a new .exe<br>
<br><code>"/path/to/exe"</code><br>
<br>
To enable <a href="https://github.com/FeralInteractive/gamemode">Gamemode</a> use this steam argument:

```bash
gamemoderun %command%
```

<br>
Running native games on steam with nvidia when in hybrid mode (having two GPUs, usually an intel igpu and nvidia dgpu).
Use this steam argument to force the game to use your nvidia gpu:

```bash
__NV_PRIME_RENDER_OFFLOAD=1 __GLX_VENDOR_LIBRARY_NAME=nvidia %command%
```

These can also be used as eviromental variables outside of steam.
<br>
<br>
To enable Gamescope use:

```bash
gamescope -W 1920 -H 1080 -r 60 -fullscreen -- %command%
```
<br>
<br>
If you want to expose your NVIDIA gpu (usually needed only to take advantage of nvidia techs) use:

```bash
PROTON_HIDE_NVIDIA_GPU=0 PROTON_ENABLE_NVAPI=1
```
<br>
<hr>

##  Cyberpunk 
<b>Steps:</b><br><br>
Add version to libraries in winecfg via either protontricks or stl
<br><br>
<b>Steam Arguments:</b> 
```bash
WINEDLLOVERRIDES="winmm,version=n,b" %command% --launcher-skip -skipStartScreen -modded
```
Current

```bash
WINEDLLOVERRIDES="winmm" PROTON_HIDE_NVIDIA_GPU=0 PROTON_ENABLE_NVAPI=1 __NV_PRIME_RENDER_OFFLOAD=1 __GLX_VENDOR_LIBRARY_NAME=nvidia %command% --launcher-skip -skipStartScreen -modded
```
<hr>


##  Skyrim SE 
Guide: <a href="https://parilia.github.io/a/gaming/modding-skyrim-linux">https://parilia.github.io/a/gaming/modding-skyrim-linux</a><br><br>
<b>Steps:</b><br><br>
For Modding use stl and mod organiser, make sure skse is installed before installing MO2 through stl. <br>
Make a mod from the skse data folder and install it on MO2.<br>
install xact and xact_x64 through stl
<hr>

##  Fallout 4 
<b>Steps:</b><br><br>
Essentially the same steps as Skyrim : <br><br>
For Modding use stl and mod organiser, make sure f4se is installed before installing MO2 through stl. <br>
Make a mod from the f4se data folder and install it on MO2.<br>
install xact and xact_x64 through stl
<hr>

##  Dawn of War Soulstorm
<b>Steps:</b><br><br>
Use Steam Tinker Launch to enable large address aware. 
<br><br>
<b>Modding:</b><br><br>
Ultimate Apocalypse: <a href="https://parilia.github.io/a/gaming/ua-linux">https://parilia.github.io/a/gaming/ua-linux</a><br>
Unification: Untested thus far but instaling through bottles should work.<br>
Others: Using bottles to install should work. 
<hr>

## Sins of a Solar Empire: Rebellion
<b>Path to mod directory:</b>
<br><br><code>/.steam/steam/steamapps/compatdata/204880/pfx/drive_c/users/steamuser/Documents/My Games/Ironclad Games/Sins of a Solar Empire Rebellion/Mods-Rebellion v1.85</code>
<br><br>
<b>Steam Arguments:</b> 
```bash
PROTON_LARGE_ADDRESS_AWARE=1 WINE_LARGE_ADDRESS_AWARE=1 %command% /nolauncher
```
<hr>

## DeepRock Galactic
<b>Steps:</b><br><br>
Use GE Proton, disable mouse smoothing ingame
<br><br>
<b>Steam Arguments:</b> 
```bash
gamemoderun PROTON_ENABLE_NVAPI=1 %command%
```
