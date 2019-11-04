# FrameCount
Tool to help measure FPS and input lag.

Implemented with Unreal Engine 4.23 in a Blueprint only project.

## Usage

1. Run FrameCount
2. Record the display, mouse, and keybaord with a high speed camera (running at a frame rate above what you are measuring)
3. Press spacebar or left mouse button.

Scrub through the high speed video you recorded and see if every frame rendered appears on the display.

* Is every frame rendered by FrameCount displayed? If not, the game is running at a higher rate than the display can handle.
* How many frames appear between input event (spacebar or left mouse button down) and the input event registering on the screen? Divide this
count by your high speed camera frame rate to determine the input lag in seconds (+/- one camera high speed camera frame).

