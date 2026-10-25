# Infinite Cabbage Cruncher 3D

A static browser game packaged for deployment through GitHub and Render.

## Deploy with GitHub + Render

1. Create a GitHub repository, for example `cabbage-muncher`.
2. Upload `index.html`, `render.yaml`, and `README.md` to the repository root, then commit the files.
3. Open the [Render dashboard](https://dashboard.render.com/).
4. Choose **New → Blueprint**, connect your GitHub account if asked, and select the repository.
5. Render reads `render.yaml` and creates the static site. Apply the Blueprint and wait for the service to become **Live**.

The site is plain HTML, CSS, and JavaScript; it does not require a server-side build or backend. The game loads Tailwind CSS, Three.js, Font Awesome, and the Outfit font from external CDNs, so a working internet connection is required for those resources.

## Save data and leaderboard

The current game saves the selected username and each player's cabbage score in the browser's `localStorage`. This means saves are local to that browser/device and the leaderboard is a solo/local leaderboard—not a shared online leaderboard. Publishing the site online does not add multiplayer or cross-device account sync.
