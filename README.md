# Bloom & Boom

An original mobile-first 3D flower workshop. Walk freely with the touch joystick or WASD/arrow keys. Gather flowers in the garden, turn two flowers into one bouquet at the workshop, sell bouquets at the market, and upgrade your business. Stations work automatically while nearby; the action button gives an immediate extra action. Drag on the world to adjust the camera.

Inspired by the satisfying gather → process → sell → upgrade loop of casual mobile tycoon games. All geometry and game code are original; no assets were copied.

## Run

Serve the repository root over HTTP (`python3 -m http.server 8000`) or open the GitHub Pages deployment. JavaScript modules and service workers require a secure hosted origin for installation. Chrome on Android can install the PWA from its menu **Add to Home screen → Install**. It works offline after first successful load. Save data lives on the device in localStorage; there is no account sync or real-money earning.

If WebGL is unavailable, a station travel view preserves the full collect/process/sell loop. The full-screen game uses WebGL without external 3D dependencies.
