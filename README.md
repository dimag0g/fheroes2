This is a port of Free Heroes 2 (free implementation of Heroes of Might and Magic 2 engine) to Nintendo Switch.
It's a homebrew app, so you need to be running custom firmware for it to work.


[1] BUILDING
------------

If you're targeting Nintendo Switch, make sure you're using the `switch` branch. The `master` branch contains changes which are not specific to Switch and could be used on other platforms.

You will need to install the [devkitPro](https://devkitpro.org/) toolchain. Make sure to include the following packages:

    libnx switch-sdl2_image switch-sdl2_mixer switch-sdl2_ttf

Then follow the usual steps to build Free Heroes 2.

If you don't intend to do any coding and just want to play, grab the latest [release](https://github.com/dimag0g/fheroes2/releases) instead.


[2] SETUP
---------

You will need a copy of the official game to run this port.

Free Heroes 2 root directory is hardcoded as `/switch/fheroes2`. Put the game files there (specifically `ANIM`, `DATA`, `MAPS` and `MUSIC` folders),
then copy over the `files` directory, as well as `fheroes2.nro`. `ANIM` and `MUSIC` folders are optional: you can play without any music or movies.
If you don't have the `ANIM` folder, create it and copy whatever `*.smk` files you have from `DATA` to `ANIM`.


In the end you should have the following directory tree on your SD card:

    switch
     |
     +-- ...
     +-- fheroes2  <--- this is the game directory
         |
         +--- anim
         +--- data
         +--- files
         +--- maps
         +--- music
         +--- fheroes2.nro


[3] RUNNING
-----------

This build of Free Heroes 2 was tested on 10.2.0|AMS 0.14.4|S (FAT32). exFAT is not recommended.
Alternative controllers (keyboards, mouses, etc.) might work but weren't tested.

Working controls are:
- Touchscreen - emulates mouse, including dragging
- L-stick - move mouse cursor
- R-stick/D-pad - scroll
- A - left mouse click
- B - Right mouse click
- X - Escape
- Y - Enter
- (+) - Cast spell
- (-) - End turn
- R - Cycle through towns
- L - Cycle through heroes


[4] TODO
--------

Here's a list of known bugs / missing features, approximately in order of priority. Don't bother reporting those as issues.

- videos have wrong aspect ratio
- locales are not supported


The game icon was downloaded from [this page](https://iconarchive.com/show/mega-games-pack-28-icons-by-3xhumed/Heroes-II-of-Might-and-Magic-2-icon.html)
with the following copyright notice:

>Artist: Exhumed

>License: CC Attribution-Noncommercial-No Derivate 4.0

>Commercial usage: Not allowed


