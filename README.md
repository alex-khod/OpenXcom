# OpenXcom [![Workflow Status][workflow-badge]][actions-url]

[workflow-badge]: https://github.com/OpenXcom/OpenXcom/workflows/ci/badge.svg
[actions-url]: https://github.com/OpenXcom/OpenXcom/actions

OpenXcom is an open-source clone of the popular "UFO: Enemy Unknown" ("X-COM:
UFO Defense" in the USA release) and "X-COM: Terror From the Deep" videogames
by Microprose, licensed under the GPL and written in C++ / SDL.

See more info at the [website](https://openxcom.org)
and the [wiki](https://www.ufopaedia.org/index.php/OpenXcom).

Uses modified code from SDL\_gfx (LGPL) with permission from author.

## Branch readme
This is fork from Meridian's OXCE branch (currently 7.9.18.0), intended for small lazy QoL features, mainly around X-Com Files / XPiratez - may not work properly with other mods.

Features:
- View UFOPaedia from tech tree viewer on right click (RMB)
- Hotkeys for sorting soldier screens (1234 = Battlescape center-on-enemy sort by Agent type, TU, Health, Accuracy, 12 - PST/PSK in psi-lab)
- Default value for scientists on a new project, as fixed 0.2 ratio of the project cost.
- Same 1234 hotkeys for Grenade prime on dialog.
- CTRL+RMB to pre-prime grenades instantly, without dialog, while in pre-battle equipment screen.
- Hotkey for "soldier transformations" screen, T.
- Shift+RMB to remove armor on soldier armor screen
- Ctrl+RMB to view soldier stats from craft screen.
- Experience gained "marks" next to soldier names in battlescape. (+ any, - melee, * psi).
- RMB to view target base's sell screen on Transfer screen (sometimes helps if all prisons are full).
- Bigger limit on dogfight speed (repetitive ones get annoying).
- Multiple interceptors targeting UFOs instead of escorting (CTRL+Click on confirmation screen).
- Hotkey for skipping walk animation (STR_SKIP_WALK_CYCLE key, home by default).

## Usage
Install OXCE. Take .exe from releases section or build one yourself. Put it into installation folder.

## Development

OpenXcom requires the following developer libraries:

- [SDL](https://www.libsdl.org) (libsdl1.2)
- [SDL\_mixer](https://www.libsdl.org/projects/SDL_mixer/) (libsdl-mixer1.2)
- [SDL\_gfx](https://www.ferzkopp.net/wordpress/2016/01/02/sdl_gfx-sdl2_gfx/) (libsdl-gfx1.2), version 2.0.22 or later
- [SDL\_image](https://www.libsdl.org/projects/SDL_image/) (libsdl-image1.2)
- [yaml-cpp](https://github.com/jbeder/yaml-cpp), version 0.5.3 or later

The source code includes files for the following build tools:

- Microsoft Visual C++ 2010 or newer
- Xcode
- Make (see Makefile.simple)
- CMake

It's also been tested on a variety of other tools on Windows/Mac/Linux. More
detailed compiling instructions are available at the
[wiki](https://ufopaedia.org/index.php/Compiling_(OpenXcom)), along with
pre-compiled dependency packages.
