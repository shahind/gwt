LiftLog — simple workout tracker PWA

FILES
- index.html: the app UI and JavaScript. No libraries or build step required.
- manifest.webmanifest: installable PWA metadata.
- sw.js: offline app-shell cache.
- icon-192.png and icon-512.png: install icons.

USE
Open index.html in a browser to use it. Workout entries are stored in that browser's localStorage on that device.
The app includes Tuesday Upper A, Thursday Upper B, Saturday Upper C, and Sunday Legs by default.
Each set has weight, reps, optional RIR, a completion checkbox, and a rest timer. Compound lifts default to 3 minutes; isolation/core exercises default to 2 minutes. Checking a set starts its rest timer if more sets remain.

INSTALL AS A PWA
For the browser's Install/Add to Home Screen option and offline caching, serve or host the folder over HTTPS (or localhost). Service workers generally do not run when opening the file directly with file://.
For example, upload all files to a static host such as GitHub Pages, or test locally with a simple server.

DATA AND BACKUP
Data stays on this device/browser and is not synced to a cloud account. Use the Export CSV button periodically to back up training logs. Clearing site data or switching browsers/devices can remove access to locally stored entries.
