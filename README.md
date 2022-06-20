# Moonscript Template for Love2D
Barebones set up for love2d games using mooonscript.

Run `./tup monitor` to automatically compile the following upon change:
* `.asesprite` -> `.png`
* `.moon` -> `.lua`
* `.tmx` -> `.lua`

# System requirements
You must have the following installed:
1. Lua  

2. [Moonscript](https://moonscript.org/)(it must be avilable in `PATH`)  

3. [Tup](https://gittup.org/tup/)  
This is used to watch changes on the file system and compile when the following are changed: 
   * `.asesprite`
   * `.moon`
   * `.tmx`


# Included libraries
These can be pulled out depending on what's needed. They're pulled in as git submodules to make them easy to remove/update/whatever.

* [Hump](https://github.com/HDictus/hump
)
* [Simple Tiled Implementation](https://github.com/karai17/Simple-Tiled-Implementation
)
* [Windfield](https://github.com/a327ex/windfield
)

# Directory Structure
## `/src`
All the source code for the game goes here.

## `/assets`
Directory for any static assets the game needs.

### `/assets/maps`
Maps made in Tiled.

### `/assets/sprites`
Graphics. Will process asesprite files automatically.

### `/assets/sound`
Any sound files.

## `/lib`
Git submoduled libraries that one might want.

# TODO
- [ ] Add tup for Tiled files(tmx, tsx)
- [ ] Makefile for compiling
- [ ] Hot reloading for:
  - [ ] Code
  - [ ] Assets
- [ ] REPL for running commands as the game is running
