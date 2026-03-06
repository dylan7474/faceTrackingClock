# faceTrackingClock

A browser-based, cyberpunk-style 3D digital clock that responds to head movement.

The app renders voxel-like digits in a faux-3D scene and uses MediaPipe face detection to tilt the camera view based on your face position. If camera tracking is not enabled, mouse movement can be used as fallback control.

## What this application is

`faceTrackingClock` is a single-page web experience built with plain HTML/CSS/JavaScript. It combines:

- A live digital clock (`HH:MM:SS`)
- A stylized holographic interface (stars, HUD ring, animated floor)
- Optional face-tracking controls via webcam (MediaPipe)
- Mouse-driven parallax controls as fallback

## Basic controls

- **Move mouse**: Rotates the 3D stage (default behavior)
- **Engage Neural Link button**: Requests webcam permission and enables face-tracking control
- **Allow camera access** (browser prompt): Required for face tracking
- **Deny/disable camera**: App remains usable with mouse control

## Build / Run instructions

No build step is required.

1. Clone the repository.
2. Serve the folder with any static web server.
3. Open `index.html` in a modern browser.

Example local server options:

```bash
# Python 3
python3 -m http.server 8080

# Node (if installed)
npx serve .
```

Then visit `http://localhost:8080` (or the port shown by your server).

> Note: A secure context may be required by some browsers for camera access (localhost is generally allowed).

## Short roadmap

- Add a settings panel for sensitivity, theme colors, and motion smoothing
- Add a camera calibration step for better tracking stability
- Add optional 12-hour/24-hour format toggle
- Add a low-power mode for reduced visual effects
- Package as a simple PWA for installable desktop/mobile usage
