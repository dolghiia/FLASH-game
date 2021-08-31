FLASH is a game built in Python using the pygame library. This game was developed with a few others I would like to give credit to. Danny, Glenn, Jace (Thank you!).
It is the latest working build, please check all the requirements before attempting to run.

Some features of the game include:

FIRST-PERSON

The most unique aspect of the game is the first-person perspective. This is done using a custom raycasting engine developed solely for this game. This translates an internal 2D map to a
'3D' perspective for the user, which immerses the user in the objective of the game.


RANDOM MAP GENERATION

The map is generated according to an algorithm developed by our team that changes the exits of the map and the pickups the user can get. This makes the game replayable, as each 
playthrough the user goes through is different from the last.


RECORDED STATS

Every run-through of the game is recorded in a text file in the game, so the user has the option of competing against themselves or friends. The game's run-through is recorded according to
the time it took to complete the game, the date the run-through occured on, and the difficulty it was played on.


ENEMY AI & CUSTOM DIFFICULTY

The main enemy of the game takes several actions to stop the user from completing their objective. The user must take different actions in response to the enemy's movements to avoid
losing the game. Most of these are outlined in the in-game documentation, however some aspects are unclear to provide a more scary atmosphere for the user. Besides hiding from most noises,
the user should also use their flashlight to shine away shadows that look like the monster. Additionally, one noise indicates the user has lost battery power, so the user does not need to
hide for this enemy action. The user has one win condition, while the enemy has several. This makes the game relatively difficult, so the user has the option to change the difficulty. 


CUSTOM SETTINGS

The game also features custom settings for the game, including the previously mentioned difficulty, controls, graphics, and whether the game will be played in fullscreen or not. The 
controls for the game depend on whether the user wants to use keyboard or mouse to control the camera, graphics change how much detail is rendered, and fullscreen determines whether the
game is in fullscreen or not (NOTE: fullscreen is recommended for most systems).


Restrictions

The most apparent restriction of the game is that the user's perspective can't be moved up or down. This is a result of the raycasting engine used, and can't be changed without increasing
the resources the game takes, and increasing the time taken to create the game's assets and engine. Besides this restriction, another is found in the engine's method of rendering non-wall
objects, as transparent pixels are still rendered, so the user may see a dark rectangle around the main image. This has little effect on gameplay, but is still a restriction none the less.



Known Errors

The only 2 known errors occur if the user enters ctrl + c on their keyboard while the game is running, and if the user selects a graphic setting that is too high for their hardware. The
python compiler may produce a run-time memory error when rendering the user's perspective, as it could run out of the available memory if its image quality is too high. For this reason
it's of utmost importance that the user doesn't select a graphic setting that is too high for their computer's hardware.



Implementation Details

1. Turn on your computer
2. Install the Pygame module, this can be done (assuming the user's OS is Windows 10) by opening command prompt and typing 'python3 -m pygame.examples.aliens'
3. Open the Python shell
4. Type in 'import pygame' to test if the Pygame module is installed
5. Click "File", then "Open" near the top of the shell window, and select the FLASH folder, then click the FLASH_main.py
6. Click the open button next to the file name
7. Click F5 on the keyboard to start the program 


Additional Files

For other python files, the game requires FLASH_characters.py, FLASH_inanimates.py, FLASH_menu.py, FLASH_primarySettings.py, FLASH_rendering.py, in addition to FLASH_main.py. Non-asset 
files include the current file, and FLASH_Scores.txt. For assets, assuming the folders are complete, the game requires the folders FLASH_Environment, FLASH_InteractiveAssets, 
FLASH_JumpScare, FLASH_MenuAssets, FLASH_Music, and FLASH_SoundEffects. Each folder contains different assets, which will be outlined now:

----------------FLASH_Environment----------------

FLASH_Escape.png
FLASH_Pause.png

--------FLASH_RenderedElements

FLASH_Background.png
FLASH_Door.png
FLASH_Fog.png
FLASH_MaxWallDistance.jpg
FLASH_Wall.png

--------FLASH_UI

FLASH_Battery0.png
FLASH_BatteryFull.png
FLASH_BatteryLow.png
FLASH_BatteryMed.png
FLASH_Key.png

-------------FLASH_InteractiveAssets-------------

--------FLASH_Flashlight

FLASH_FlashlightHalfway.png
FLASH_FlashlightOff.png
FLASH_FlashlightOn.png

--------FLASH_Monster

FLASH_Hallucination.png
FLASH_ShadowMonster.png

--------FLASH_Pickups

FLASH_Battery.png
FLASH_Key.png	(DIFFERENT FILE FROM FLASH_UI'S FLASH_Key.png FILE)

-----------------FLASH_JumpScare-----------------

FLASH_01.png
FLASH_02.png
FLASH_03.png
FLASH_04.png
FLASH_05.png
FLASH_06.png
FLASH_07.png
FLASH_08.png
FLASH_09.png
FLASH_10.png

FLASH_11.png
FLASH_12.png
FLASH_13.png
FLASH_14.png
FLASH_15.png
FLASH_16.png
FLASH_17.png
FLASH_18.png
FLASH_19.png
FLASH_20.png

FLASH_21.png
FLASH_22.png
FLASH_23.png
FLASH_24.png
FLASH_25.png
FLASH_26.png

-----------------FLASH_MenuAssets----------------

FLASH_Icon.png
FLASH_Over.png
FLASH_Win.png

--------FLASH_Backgrounds

FLASH_CreditsScreen.png
FLASH_HowToPlayControls.png
FLASH_HowToPlayScreen.png
FLASH_MenuBackground.png
FLASH_SettingsMenu.png

--------FLASH_Buttons

FLASH_Back.png
FLASH_BackHighlighted.png
FLASH_Blackbox.png
FLASH_Controls.png
FLASH_CreditsHighlighted.png
FLASH_Easy.png
FLASH_EasyHighlighted.png
FLASH_Exit.png
FLASH_ExitHighlighted.png
FLASH_Graphics.png
FLASH_GraphicsHighlighted.png

FLASH_Hard.png
FLASH_HardHighlighted.png
FLASH_Help.png
FLASH_HelpHighlighted.png
FLASH_High.png
FLASH_HighHighlighted.png
FLASH_KeybindsHighlighted.png
FLASH_Keyboard.png
FLASH_KeyboardHighlighted.png
FLASH_Low.png
FLASH_LowHighlighted.png

FLASH_Medium.png
FLASH_MediumHighlighted.png
FLASH_Mouse.png
FLASH_MouseHighlighted.png
FLASH_Next.png
FLASH_NextHighlighted.png
FLASH_Normal.png
FLASH_NormalHighlighted.png
FLASH_Options.png
FLASH_OptionsHighlighted.png
FLASH_Start.png

FLASH_StartHighlighted.png
FLASH_TickedBox.png
FLASH_TickedHighlighted.png
FLASH_Tutorials.png
FLASH_TutorialsHighlighted.png
FLASH_Unticked.png
FLASH_UntickedHighlighted.png

--------FLASH_Logos

FLASH_Logo.png
FLASH_Title.png

-------------------FLASH_Music-------------------

FLASH_chase.ogg

----------------FLASH_SoundEffects---------------

FLASH_ding.wav
FLASH_discovery.wav
FLASH_flashlightOn.wav
FLASH_gameOver.ogg
FLASH_jumpscare.ogg

FLASH_lowMonster.wav
FLASH_monsterStep.ogg
FLASH_shock.wav
FLASH_steps.wav
FLASH_swoosh.ogg
