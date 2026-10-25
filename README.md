# HandFrame Studio

**Control, create and play with hand gestures.**

HandFrame Studio is a Windows desktop application that turns your webcam into a hand-tracking interface for mouse control, drawing, music and photo puzzles.

## Video Demo

[▶ Watch the HandFrame Studio demo](https://github.com/pooyaHajiSadeghi/HandFrame-Studio/blob/main/HandFrameStudio_Promo.mp4)

Open the link above to view the demo on GitHub. If playback is unavailable on the file page, download the MP4 and open it locally.

[Browse releases](https://github.com/pooyaHajiSadeghi/HandFrame-Studio/releases)

Use the installer from the release assets to install the application. The repository ZIP is not the Windows installer.

## Installation

1. Download `HandFrameStudio_Setup_1.0.0.exe` using the link above.
2. Run the installer and follow the setup wizard.
3. Choose an installation folder and complete installation.
4. Launch HandFrame Studio.
5. Allow camera access when requested and select a tool from the sidebar.

## Features

### Mouse Control

Move the Windows pointer and perform mouse actions using hand gestures.

- Index finger: move the pointer.
- Index and middle fingers raised in a V sign: left-click.
- Thumb and middle finger gesture: right-click.
- Hold a thumb-and-index pinch: drag.
- Index, middle and ring fingers raised: scroll.
- Press **F8** to enable or disable mouse control.

Follow the on-screen gesture guide. Mouse control turns off when you leave its page.

### Hand Drawing

Draw with your index finger, choose colors, adjust brush size, switch between brush and eraser, undo changes and save your artwork as a PNG image.

### Hand Music

Use tracked hand gestures to play musical notes and drum sounds. Choose an instrument or mode, adjust volume and tempo, and record and save audio as a WAV file.

### Photo Puzzle

Frame a photo with your hands and solve a shuffled puzzle. Point to highlight a tile, pinch to grab it, move your hand to drag it, and release to drop it. The interface shows progress, moves, time and score.

## Getting Started

- Use a working webcam with Windows camera access enabled.
- Keep your hands inside the camera view and use even lighting.
- Leave enough space between your hands and the camera for fingers to be visible.
- Start with one tool and follow its on-screen instructions.
- Use **F8** to pause pointer control when needed.

Only one tool is active at a time.

## Troubleshooting

**The camera does not open**  
Check Windows camera privacy settings, close other applications using the webcam and restart HandFrame Studio.

**Hand tracking is unstable**  
Improve lighting, keep your hands visible and avoid fast movements or a cluttered background.

**Pointer control is inactive**  
Open Mouse Control and press **F8**. Check the on-screen status and gesture guide.

**Music is silent**  
Check Windows output volume, the selected audio device and the application's volume setting.

## Technical Overview

The application combines a Python backend with an HTML, CSS and JavaScript dashboard hosted through pywebview. MediaPipe provides hand landmarks; OpenCV handles camera frames and image processing. Other components include NumPy, Pillow, PyAutoGUI, pynput and sounddevice.

For architecture, libraries and implementation details, see [Technical Documentation](README_TECHNICAL.md).

## About This Repository

This repository provides the Windows installer, usage documentation and demonstration media. Application source code is not included here.

## Developer

**Pooya Haji Sadeghi**  
[GitHub Profile](https://github.com/pooyaHajiSadeghi)
