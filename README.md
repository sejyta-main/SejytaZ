# Bloom & Boom

An original mobile-first 3D flower workshop. Walk freely with the touch joystick or WASD/arrow keys. Gather flowers in the garden, turn two flowers into one bouquet at the workshop, sell bouquets at the market, and upgrade your business. Stations work automatically while nearby; the action button gives an immediate extra action. Drag on the world to adjust the camera.

Inspired by the satisfying gather → process → sell → upgrade loop of casual mobile tycoon games. All geometry and game code are original; no assets were copied.

## Run

Serve the repository root over HTTP (`python3 -m http.server 8000`) or open the GitHub Pages deployment. JavaScript modules and service workers require a secure hosted origin for installation. Chrome on Android can install the PWA from its menu **Add to Home screen → Install**. It works offline after first successful load. Save data lives on the device in localStorage; there is no account sync or real-money earning.

If WebGL is unavailable or loses its context, the game switches to a mobile-friendly illustrated world with the same movement, customers and production loop. The 🎨 button lets you choose a graphics mode. The WebGL world and the illustrated renderer have no external runtime dependencies.

## Interaction update

Flowers visibly leave the beds, processed bouquets travel through the workshop, and sale coins move from the market. Carried inventory stacks on the character. Loose petals bounce under gravity and flowers regrow. The character accelerates smoothly and collides with garden beds, worktables, market counter and upgrade board. This is a lightweight custom game simulation, not a general-purpose rigid-body physics engine.

## Greenhouse story update

Nine story chapters follow Mira and Eli from reopening the stall to preparing for the spring festival. Fulfill town orders for reputation and bonuses, unlock the berry orchard, gather berries, cook jam, and sell both bouquets and jars. The world now includes the orchard gate, kitchen, customers, winding paths and moving products. An oven upgrade accelerates cooking. Existing local saves carry forward.

## Customer and crew update

Customers line up at the market with a specific bouquet or jam request. Their patience runs out in game time and unmet orders cost reputation. Serving promptly pays a tip. Tap the money display for the income ledger and current earnings rate. Hire a flower picker, florist, berry picker, chef and cashier separately; staff work while you move through the world. Customers, staff, register cash, terrain, and the shop frontage are visible in the 3D world. The simulation pauses while a menu is open and does not penalize you for being away from the app.

## Graphics recovery

The old emoji station grid has been replaced by an illustrated world with a following camera, depth-sorted buildings, crops, staff and customers. On devices with WebGL the original low-poly world remains available. A transient rendering problem no longer permanently disables the game because the illustrated mode takes over. Inventory, progress and earnings stay in the same save.

After the story, repeatable shifts ask you to serve an increasing number of customers before two leave. A successful shift pays a bonus; two missed customers restart that shift. The counter and bonus appear in the mission HUD and earnings panel.
