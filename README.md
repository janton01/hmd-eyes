# hmd-eyes

Building blocks for eye tracking in Augmented Reality `AR` and Virtual Reality `VR` or more generally Head Mounted Displays `HMD`.

## Setup

1. Make sure that you have [Pupil Service](https://github.com/pupil-labs/pupil/releases/latest) on a Linux, macOS, or Windows 10 machine.
2. Open `Assets/scene/Calibration.unity` with the Unity3d Editor (Unity 5.5 and above).
3. Select the PupilGaze GameObject in Unity Hierarchy.

4. Connection
	* **Local** - use this setting if your HMD and your Pupil add-on are connected to the same computer.
		1. In Unity's Inspector select `Settings>Pupil App>Local`
		2. Click on the Browse button. Navigate to Pupil Service - pupil_service.exe.
		
6. Confirm connection - Make sure that the plugin status (below the Pupil Labs logotype) displays the word "connected" and that both of the eye icons are green. The green eye icons signify that the eye processes are running.

## Calibration


2. Press Play in Unity and wait until you have established a working connection with your Pupil App.
3. Calibrate - Give focus to the main Unity3d window and press c on the keyboard or the `Calibrate` button in the plugin GUI.
4. Put your headset on and look at the center of each marker shown in your HMD. #The number of markers varies depending on your calibration #mode.

Note: The ideal setup for calibration may vary using different headsets. For optimal calibration results I suggest some experimenting with the hardware settings of your HMD device such as the eye distance from the lens, inter eye distance, a steady mount position.

## Data access

1. 2D
	1. You can access the 2d gaze point in Unity3d with `GetEyeGaze2D (GazeSource.BothEyes)`.
2. 3D
	1. `Pupil.values.GazePoint3D`
	2. `Pupil.values.GazeNormals3D`
	3. `Pupil.values.EyeCenters3D`

## Connect

Chat with the hmd-eyes community on [Discord](https://discord.gg/PahDtSH).

Join the [google group](https://groups.google.com/forum/#!forum/hmd-eyes) to discuss ideas and stay updated. 
