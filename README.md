# Gaming
A place for all my gaming related stuffs
<!--
<hr>
<h3>Game</h3>

<b>Steps:</b><br><br>

<br><br>
<b>Steam Arguments:</b><br><br>
<code>Arguments go here</code>

-->
<h2>Useful Info</h2>
Move default pfx location on steam<br>
<br><code>STEAM_COMPAT_DATA_PATH= %command%</code><br>
<br>
the target path needs to be inside quotations<br>
<br><code>"/path/to/exe"</code>

<h2>Steam</h2>
<h3>Cyberpunk</h3>

<b>Steps:</b><br><br>
Add version to libraries in winecfg via either protontricks or stl
<br><br>
<b>Steam Arguments:</b><br><br>
<code>WINEDLLOVERRIDES="winmm,version=n,b" __GL_SHADER_DISK_CACHE_SKIP_CLEANUP=1 %command% --launcher-skip -skipStartScreen -modded</code>
<hr>
<h3>Skyrim SE</h3>
Guide: <a href="https://parilia.github.io/a/gaming/modding-skyrim-linux">https://parilia.github.io/a/gaming/modding-skyrim-linux</a><br><br>
<b>Steps:</b><br><br>
For Modding use stl and mod organiser, make sure skse is installed before installing MO2 through stl. <br>
Make a mod from the skse data folder and install it on MO2.<br>
install xact and xact_x64 through stl
<hr>
<h3>Fallout 4</h3>
<b>Steps:</b><br><br>
Essentially the same steps as Skyrim : <br><br>
For Modding use stl and mod organiser, make sure f4se is installed before installing MO2 through stl. <br>
Make a mod from the f4se data folder and install it on MO2.<br>
install xact and xact_x64 through stl
<hr>
<h3>Dawn of War Soulstorm</h3>
<b>Steps:</b><br><br>
Use Steam Tinker Launch to enable large address aware. 
<br><br>
<b>Modding:</b><br><br>
Ultimate Apocalypse: <a href="https://parilia.github.io/a/gaming/ua-linux">https://parilia.github.io/a/gaming/ua-linux</a><br>
Unification: Untested thus far but instaling through bottles should work.<br>
Others: Using bottles to install should work. 
<hr>
<h3>Sins of a Solar Empire: Rebellion</h3>
<b>Path to mod directory:</b>
<br><br><code>/.steam/steam/steamapps/compatdata/204880/pfx/drive_c/users/steamuser/Documents/My Games/Ironclad Games/Sins of a Solar Empire Rebellion/Mods-Rebellion v1.85</code>
<br><br>
<b>Steam Arguments:</b><br><br>
<code>PROTON_LARGE_ADDRESS_AWARE=1 WINE_LARGE_ADDRESS_AWARE=1 %command% /nolauncher</code>

