# Unity-GameSense-Project
Unity ver. 2019.2.7f2
2019.1 version and standalone available for download [here.](https://steelseries.box.com/s/x54w08fbinxhxrywigyisotybq8v8dal)

The intention of this repo is to supplement the instructions and documentation listed for SteelSeries [GameSense SDK](https://github.com/SteelSeries/gamesense-sdk) and [Unity GameSense Client](https://github.com/SteelSeries/unity-gamesense-client).

unity-gamesense-client is included as a submodule of this repo, so remember to: 

`git submodule update --init --recursive` 


### Features
Here you will find example code to help you understand and utilize the Unity GameSense client in your own Unity projects. 
For more information about GameSense, visit the repo [here.](https://github.com/SteelSeries/gamesense-sdk)


Included in this repo is a simple Unity project with two scenes. 
- **GSPrefabScene** showcases the use of the GameSenseManager Prefab for handling GameSense events.
	- Ranged-event is triggered using the up-down buttons or arrow keys
		provided handlers:
		- RangedColorHandler - Changes keyboard main zone color according to the ranged-event value
		- RangedScreenHandler - Updates the screen with different readouts depending on ranged-event-value
		- GradientColorHandler - Changes the numpad zone color using a gradient according to the ranged-event value
	- Binary-event is triggered with the toggle button
		provided handlers:
		- StaticColorHandler - Switches the mouse logo zone LED on and off with toggle
		- StaticScreenHandler - Flashes an image on OLED screens when toggle is pressed
		- TactileHandler - Sends a tactile buzz to supported devices
- **GSScriptedScene** mirrors the functionality of GSPrefabScene, but uses a script-only approach.
	- Ranged-event is triggered using the up-down buttons or arrow keys
		provided handlers:
		- RangedColorHandler - Changes keyboard main zone color according to the ranged-event value
		- ScreenHandler - Updates the screen with different readouts depending on ranged-event-value
	- Binary-event is triggered with the toggle button
		provided handlers:
		- StaticColorHandler - Switches the mouse logo zone LED on and off with toggle
		- TactileHandler - Sends a tactile buzz to supported devices
