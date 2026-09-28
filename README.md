# Bloom & Boom — Garden Hotel

An original mobile PWA blending an expanding hotel management game with the earlier flower workshop. The current game starts at `index.html`; `classic.html` preserves the earlier flower/berry business and its save. Open it via the Map menu.

## Play

Move with the touch joystick, WASD or by tapping a point in the world. Welcome guests at reception, assign available rooms, collect their payment at checkout, clean rooms, and build the next room along the corridor. Each new room physically extends the hotel. Guests walk to reception and their rooms, wait with a patience timer, stay and check out. A dirty room cannot be occupied until cleaned.

The greenhouse grows flowers; two flowers make a bouquet. Decorate guest rooms for better earnings, supply the flower lounge, cook garden jam for the café, and open a bathroom and pool. Hire a receptionist, cleaner, gardener, florist and attendant to automate different stages. Buy room levels and facilities, handle VIPs, rainy days and festival crowds, and complete repeatable timed service shifts. The 11-chapter original story links Mira's revived greenhouse to a garden hotel. Existing Bloom & Boom balances and inventory migrate once on first launch; the classic game remains accessible.

The main renderer is real-time Three.js WebGL with modeled rooms, guests, moving character, lighting and shadows. If WebGL cannot initialize, the same simulation uses an illustrated Canvas 2D renderer so guests and expansion remain playable. Three.js is bundled under its MIT license in `LICENSE-three.txt`; all game content, geometry and systems are original. No advertising, purchases or network account are required.

## Install and run

Serve this directory over HTTP, for example `python3 -m http.server 8000`, or use GitHub Pages. On Android Chrome choose **⋮ → Add to Home screen → Install**. The service worker caches the game and art for offline play after its first complete load. Progress is saved in device localStorage, separate from the classic game. The game has no real money feature.

## Reference study

The Google Play description of SayGames' *My Perfect Hotel* describes a reception → room → cleaning → payment loop, staffing, upgraded rooms, bathrooms, restaurants and pools. This project adopts those broad management mechanics while using its own garden hotel story, flower supply chain, artwork, layout, prices, UI and implementation. It does not copy the reference game's assets or code.

To rebuild: `npm install` and `npm run build` in this directory. The minified bundle is checked in for GitHub Pages.
