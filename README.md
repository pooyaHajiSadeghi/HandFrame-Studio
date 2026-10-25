# HandFrame Studio

**Control, create and play with hand gestures.**

A Windows desktop application for hand-controlled photo puzzles, mouse control, drawing and music.

## Download for Windows

### [Download HandFrame Studio v1.0.0 — Windows Installer](https://github.com/pooyaHajiSadeghi/HandFrame-Studio/releases/download/v1.0.0/HandFrameStudio_Setup_1.0.0.exe)

**Windows x64 · Version 1.0.0 · Approximately 148 MiB · No Python installation required**

[View release details](https://github.com/pooyaHajiSadeghi/HandFrame-Studio/releases/tag/v1.0.0) · [All releases](https://github.com/pooyaHajiSadeghi/HandFrame-Studio/releases)

Download the **.exe installer** using the link above or from the release page's **Assets** section. GitHub's **Code → Download ZIP** and automatically generated **Source code** archives are not the Windows installer.

This repository provides the application download and user documentation.

## Install and launch

1. Download **HandFrameStudio_Setup_1.0.0.exe**.
2. Close any running copy of HandFrame Studio, then open the downloaded installer.
3. Choose the installer language.
4. Choose whether to create a desktop shortcut and select your installation folder with **Browse**.
5. Click **Install** and follow the progress and details panel.
6. If Microsoft Edge WebView2 Runtime is missing, Setup downloads and installs it from Microsoft. Internet access is needed for this step.
7. On the final page, leave **Launch HandFrame Studio** selected and click **Finish**.

After installation, open HandFrame Studio from the desktop shortcut, if selected, or the Windows Start menu.

**You do not need Python, pip, VS Code or the project source files to use the application.** Application files are included in Setup.

## Before your first session

- Connect your webcam and close other applications that are using it.
- Allow camera access for desktop applications in Windows privacy settings.
- Open **Settings** in HandFrame Studio to select the correct camera index and audio output device.
- Choose **Persian** or **English** as the application language.
- Keep your hands inside the camera view, with enough light and a clear background.

## What you can do

| Tool | Features |
| --- | --- |
| Photo Puzzle | Capture an area with two hands and solve a shuffled 3×3, 4×4 or 5×5 puzzle using pointing, pinching and dragging. |
| Mouse Control | Move the pointer, click, drag and scroll with hand gestures. Use **F8** to enable or disable control. |
| Drawing | Draw with your finger, choose colors, change brush size, erase, undo and save PNG images. |
| Music | Play piano and drums, use Free Play or Groove mode, adjust volume and tempo, and record WAV audio. |
| Dashboard | Switch tools, change device settings and use the Persian/English interface. |

## How to use the tools

### Photo Puzzle

1. Select **Photo Puzzle** from the dashboard.
2. Show both hands to the camera. Pinch your thumb and index finger on each hand and move your hands apart to create a frame.
3. Open your fingers to freeze the frame. After a five-second countdown, the captured area becomes a shuffled puzzle.
4. Point at a tile, pinch to grab it, move it to another position and open your fingers to drop it.
5. Use the difficulty selector for **3×3**, **4×4** or **5×5** grids. Changing difficulty starts a new puzzle.

### Mouse Control

1. Select **Mouse Control**.
2. Read the on-screen gesture guide before enabling pointer control.
3. Press **F8**, or use the on-screen toggle, to enable control.
4. Use the indicated gestures to move, click, drag and scroll.
5. Press **F8** whenever you want to stop gesture-based mouse control.

### Drawing

1. Select **Drawing**.
2. Raise your index finger and fold the other fingers to draw.
3. Choose a color and brush size; use the eraser or **Undo** when needed.
4. Click **Save** to choose a location and export your drawing as a **PNG**.

### Music

1. Select **Music** and choose **Free Play** or **Groove**.
2. Use the on-screen hand-gesture guide, instrument buttons or keyboard shortcuts to play.
3. Adjust the instrument preset, volume and tempo.
4. To save a performance, start recording, stop recording, then choose **Save** to export a **WAV** file.

Each recording can be up to **five minutes** long. Save drawings and recordings before leaving the active tool.


## System requirements

- **64-bit Windows**; Windows 11 is the primary tested environment.
- A webcam for hand tracking.
- An audio output device for music.
- Microsoft Edge WebView2 Runtime for the dashboard.
- Internet access if Setup needs to install WebView2.

## Troubleshooting

| Problem | What to try |
| --- | --- |
| Camera unavailable or no picture | Close other camera apps, check Windows camera permissions and select the correct camera index in Settings. |
| Hand tracking is unstable | Improve lighting, keep your hands fully visible and avoid a busy background. |
| No sound | Check Windows volume and choose the correct audio output device in Settings. |
| WebView2 installation fails | Check your internet connection, or install the [Evergreen Runtime from Microsoft](https://developer.microsoft.com/microsoft-edge/webview2/) and rerun Setup. |
| Unexpected mouse actions | Press **F8** to disable gesture-based mouse control. |
| Setup asks you to close HandFrame Studio | Exit the running application, then retry installation. |

Application logs are stored at:

```text
%LOCALAPPDATA%\HandFrame\logs\handframe.log
```

For help, [open an issue](https://github.com/pooyaHajiSadeghi/HandFrame-Studio/issues) with your Windows version, the affected tool and the error message. Review logs before sharing them and remove any personal information.

## Updates and uninstall

Download future versions from the [Releases page](https://github.com/pooyaHajiSadeghi/HandFrame-Studio/releases). Close the application before running a new installer.

To change the installation folder, uninstall the current copy first. To remove the application, use **Windows Settings → Apps → HandFrame Studio → Uninstall**, or the Start menu uninstall shortcut.

Saved drawings, audio exports, preferences and the shared WebView2 Runtime are kept.

## Developer

**Pooya Haji Sadeghi** — [GitHub](https://github.com/pooyaHajiSadeghi)
