# HandFrame Studio

**Control, create and play with hand gestures.**

A Windows desktop application for gesture-controlled photo puzzles, mouse control, drawing and music. Developed by **Pooya Haji Sadeghi**.

## Download and install

Open this repository's **Releases** page and download `HandFrameStudio_Setup_1.0.0.exe`.

1. Close any running copy of HandFrame Studio.
2. Run the installer and choose your preferred language.
3. Select the desktop shortcut option and installation folder.
4. Follow the installation progress. If Microsoft Edge WebView2 Runtime is missing, Setup downloads and installs it from Microsoft.
5. Select **Launch HandFrame Studio** on the final page.

**Python is not required on the end user's computer.** Application files are included in Setup. Internet access is required only if the WebView2 prerequisite must be downloaded.

For the portable edition, download `HandFrameStudio_Portable.zip`, extract the entire archive, and run `HandFrameStudio.exe`. Keep `_internal` next to the executable. The portable edition requires an existing WebView2 Runtime or its manual installation.

## Features

| Tool | Features |
| --- | --- |
| Photo puzzle | Create a frame with two hands, capture the area, and solve a shuffled 3×3, 4×4 or 5×5 puzzle by pointing, pinching and dragging. |
| Mouse control | Gesture-based pointer movement, clicks, dragging and scrolling, with an F8 toggle. |
| Drawing | Finger drawing, colors, adjustable brush, eraser, undo and PNG export. |
| Music | Piano and drums, Free Play and Groove modes, volume/tempo controls and WAV recording. |
| Dashboard | Persian/English UI, bundled Vazir fonts, device settings and unsaved-work prompts. |

## Requirements

- 64-bit Windows; Windows 11 is the primary tested environment.
- A working webcam for hand tracking.
- An audio output device for music.
- Microsoft Edge WebView2 Runtime for the dashboard.
- Permission to use the camera and, optionally, an internet connection for missing WebView2 components.

## Quick controls

- **F8:** enable or disable mouse control.
- **Space:** pause/resume the active puzzle, drawing or music tool.
- **Esc:** return to the home page.
- **C:** start a new puzzle.
- **Ctrl+S / Ctrl+Z:** save / undo in Drawing.
- **1–8 / A, S, D, F:** piano keys / drum pads in Music.

Use each tool's on-screen gesture guide. Save drawings and recordings before leaving a tool. Audio recording is limited to five minutes per take.

## Uninstall and updates

Close the application before reinstalling or updating. To change the installation path, uninstall the current copy first. Remove the application through **Windows Settings → Apps**, or its Start menu uninstall shortcut. Saved drawings, audio exports, preferences and the shared WebView2 Runtime are kept.

## Troubleshooting

- **Camera unavailable:** close other camera applications, check Windows camera permissions, and select the correct camera index in Settings.
- **No sound:** select the correct output device in Settings and check the system volume.
- **Missing WebView2:** install the [Evergreen Runtime from Microsoft](https://developer.microsoft.com/microsoft-edge/webview2/) and reopen the application.
- **Unexpected mouse actions:** press **F8** to disable mouse control.
- **Logs:** packaged application logs are stored in `%LOCALAPPDATA%\HandFrame\logs\handframe.log`.

A build without an Authenticode certificate is unsigned. Release checksums help verify file integrity; they do not provide publisher authentication.

## Development

Use **64-bit Python 3.10** for the provided Windows build scripts. The build process creates an isolated environment using the existing interpreter; it does not install a new Python version.

```bat
install.bat
run.bat
```

Build commands:

```bat
build_portable.bat
build_setup.bat
build_release.bat
```

`build_setup.bat` reuses an existing portable build. `build_release.bat` builds the application, NSIS Setup, documentation, manifest and SHA-256 checksums. The builder uses an installed NSIS compiler or downloads a pinned portable version and verifies its checksum.

Core technologies: Python, MediaPipe, OpenCV, NumPy, Pillow, pywebview, PyAutoGUI, pynput and sounddevice. Setup uses NSIS Modern UI 2 and Windows PowerShell for prerequisite checks.

See `requirements.txt` for dependency versions and `docs/NSIS_SETUP_FA.txt` for detailed build instructions. Third-party asset notices are bundled with the project. No project-wide open-source license is asserted by this README; the repository owner should choose one before describing the project as open source.

## Developer

**Pooya Haji Sadeghi** — [GitHub](https://github.com/pooyaHajiSadeghi)
