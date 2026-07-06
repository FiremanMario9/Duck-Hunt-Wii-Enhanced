# Duck Hunt Wii Enhanced

## Identified Functions

FUN_8001e66c
- Large gameplay/render function.
- References:
  - "FLY"
  - "AWAY"
  - "FRAMES"

FUN_8001d2bc (renamed DrawText)
- Likely renders text.
- Called with "FRAMES" string.
- 132 lines long.
- Name is tentative.

FUN_8003c794
- Reads Wii hardware timer register.
- Used when calculating FPS.

## Confirmed

✓ Ghidra imports DOL correctly
✓ Decompiler working
✓ Located FPS rendering code

## TODO

[ ] Remove FPS counter
[ ] Find controller input
[ ] Find pause menu location
[ ] Find duck state machine
[ ] Investigate third-shot "Got Away" bug
[ ] Replace music# Duck Hunt Wii Enhanced

## Functions

FUN_8001e66c
- Contains references to:
  - "FLY"
  - "AWAY"
  - "FRAMES"
- Probably gameplay + HUD.

## TODO

- Remove FPS counter.
- Find pause input.
- Find third-shot "Got Away" bug.
- Replace music.

## Progress

- Changed FUN_8001d2bc → DrawText
