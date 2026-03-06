# AGENTS.md

Guidance for AI coding agents working in this repository.

## Project overview

- This project is intentionally lightweight and currently centered around a single-page app in `index.html`.
- The app is static (no backend) and designed to run from a simple local web server.

## Tech stack

- HTML/CSS/JavaScript (vanilla)
- External browser-loaded dependencies via CDN:
  - `@mediapipe/face_detection`
  - `@mediapipe/camera_utils`

## Working agreements

- Keep dependencies minimal unless explicitly requested.
- Prefer direct, readable JavaScript over framework abstractions.
- Preserve the existing visual style unless the task asks for redesign.
- Avoid unnecessary file churn in `index.html`; keep changes targeted.

## Validation checklist

When making code changes:

1. Open the app in a browser.
2. Confirm the clock updates in real time.
3. Confirm mouse movement affects the 3D perspective.
4. If camera behavior is changed, verify webcam permission flow and fallback behavior.

## Documentation expectations

- Update `README.md` when controls, startup steps, or major features change.
- Keep roadmap items short and practical.
- If adding scripts or tools, document how to run them.

## Out of scope by default

- No backend service additions.
- No build system migration unless explicitly requested.
