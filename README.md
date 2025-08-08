# Ping Pong PWA Game

A responsive, mobile-friendly **Ping Pong** game built with HTML5 Canvas and JavaScript, now enhanced with **Progressive Web App (PWA)** support for offline play.

## Features
- Classic Pong gameplay
- Responsive layout for desktop and mobile
- Mouse/touch controls for the player paddle
- AI opponent paddle
- Offline capability via Service Worker
- Installable as a PWA with an **Install App** button
- Precache of assets for full offline functionality

## Files
- `index.html` – The main game and UI logic
- `manifest.json` – PWA manifest configuration
- `sw.js` – Service Worker for caching and offline use

## How to Run Locally
1. **Clone or download** this repository.
2. Serve files via a local HTTP server (PWA requires `http` or `https`). You can use Python’s built-in server:
   ```bash
   python3 -m http.server 8000
   ```
   or Node’s `http-server`:
   ```bash
   npx http-server .
   ```
3. Open your browser and navigate to:
   ```
   http://localhost:8000
   ```
4. Play the game! You’ll see the **Install App** button when eligible.

## PWA Installation
- On supported browsers, click the **Install App** button or use the browser’s install prompt.
- The game will be installed as a standalone app and will work offline.

## Offline Mode
- When installed or after the first visit, assets are precached by `sw.js`.
- The game remains playable without an internet connection.

## License
This project is licensed under the MIT License.
