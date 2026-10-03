# Creepshow-VR-Mod
CreepshowVRMod

CREEPSHOW VR  -  VR mod for "Creepshow" (Unity 2022.3, IL2CPP)
=================================================================

Version 0.1.13 (test build on Quest 3 VDXR).

WHAT IT DOES
------------
* Stereo VR through OpenXR (SteamVR, Meta/Oculus, Virtual Desktop, WMR...).
* First person: you are in the character's head (body hidden). The left stick walks where you look,
  the right stick turns (snap turn by default).
* Cutscenes and close-up puzzles switch to the game's own camera (you can still look around);
  you go back to first person afterwards.
* The character's flashlight beam comes from your left hand.
* The VR controllers act as a gamepad for the game's own controls and menus.
* The HUD and menus are on a screen floating in front of you.

INSTALL
-------
1. Copy thefiles from zip into the game folder (merge / overwrite).
2. Start SteamVR (or your OpenXR runtime), then start the game.

CONTROLS (gamepad layout)
-------------------------
Left stick ............... walk              Right stick ........ turn (menus / puzzles: right stick)

A ........................ A                 B .................. B

X (tap) .................. X                 Y (tap) ............ Y

Hold Y (about 1 s) ....... switch first person <-> the game's own camera view

Left / right grip ........ LB / RB           Left / right trigger LT / RT

Left / right stick click . L3 / R3           Both stick clicks .. re-centre

X + Y together ........... pause (Start)     Hold X ............. Back / View

In menus the right stick is also the d-pad.

Everything is in BepInEx\config\creepshow.vr.cfg ([Controls] = gamepad buttons).

BUTTON PROMPTS:         the game's button icon over things you can use shows on your right controller.

ITEM MARKERS:           white dots float on things you can use (gold = usable right now).

CLOSE-UP PUZZLES:       the screen lines up with the game's view - point the blue laser at the dot / spot and pull the trigger.

MENUS:                  point your right hand at the menu screen (blue laser) and pull the trigger.

IN-GAME SETTINGS MENU:  hold Y + left stick click for 1.7 s (view mode, puzzles, body, fades...).

HAND ADJUST:            hold Y + right stick click for 1.5 s.

USEFUL SETTINGS ([View] in the config)
--------------------------------------
ViewMode = FirstPerson / GameCamera   (GameCamera = watch from the game's fixed cameras)
PuzzleView = Game / FirstPerson       (close-ups use the game camera or stay first person)
EyeHeight = 0                         (0 = measured from the character's head)
FirstPersonLayers = All               (if you see odd things in first person, try Game)
GameCameraPullBack = 0.4              (game camera view: how far behind the camera you sit, metres)
ViewToggleHoldTime = 0.8              (hold Y this long to switch view; 0 = off)
[UI] PromptOnHand / PromptOffset / PromptSize / PromptScale   (the prompt on the right controller)



Uses Astien's OpenXR bridge (see BepInEx\plugins\CSVR\LICENSES). Free, non-commercial.
