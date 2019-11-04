# UE4 FrameCount
Tool to help measure FPS and input lag of a system running a UE4 based game.

The tool is implemented as a stripped down Unreal Engine 4 game in order to provide
a baseline FPS and input lag for games built on top of UE4. This may add >= 1 frame
of input lag depending on how UE4 is buffering frames.

Implemented with Unreal Engine 4.23 in a Blueprint only project.

## Usage

1. Run FrameCount
2. Record the display, mouse, and keybaord with a high speed camera (running at a frame rate above what you are measuring)
3. Press spacebar or left mouse button.

Scrub through the high speed video you recorded and see if every frame rendered appears on the display.

* Is every frame rendered by FrameCount displayed? If not, the game is running at a higher rate than the display can handle.
* How many frames appear between input event (spacebar or left mouse button down) and the input event registering on the screen? Divide this
count by your high speed camera frame rate to determine the input lag in seconds (+/- one camera high speed camera frame).

