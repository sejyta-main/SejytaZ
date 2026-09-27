# Sunny Acres

An original, responsive idle farming browser game inspired by the harvest, sell, upgrade, and expand loop. No copied assets or game code.

## Play locally

Open `index.html` in a browser, or serve this directory using `python3 -m http.server 8000` and visit `http://localhost:8000`.

Tap plots to plant and harvest. Sell crops, deliver orders, purchase land and upgrades, unlock crops with XP, and hire helpers. Progress saves automatically in browser localStorage. Growth continues while the tab is closed, but helpers work only while the game is open. Money is **in-game currency**, not withdrawable cash.

## Publishing

GitHub Pages can serve this static repository from its root directory. Select `main` / root under repository Settings → Pages.

## 3D and mobile installation

The farm is rendered with native WebGL, including draggable camera rotation and tap controls. It has no 3D library dependency. On Android Chrome, open the published HTTPS site and choose **Install app** or **Add to Home screen** from the browser menu. Chrome may also show the in-game Install button. On iPhone Safari, choose **Share → Add to Home Screen**. Installed versions work offline after the first successful load. Progress is saved per browser/device and does not sync across devices.
