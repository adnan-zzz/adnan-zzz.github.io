GOGGLE CHROMINIUM — CHROMEBOOK EDITION

This is a Chromebook-friendly installable web app (PWA), not a standalone browser engine.
It uses the Chrome browser already on ChromeOS to open websites in new tabs. It does not require Node.js or ChromeOS Developer Mode.

WHAT IT DOES
- Google search and URL navigation
- Quick links to popular websites
- Save/remove bookmarks in local browser storage
- Installable app-style window when served over HTTPS
- Service worker caches the app shell for quicker loading/offline access to the home screen

IMPORTANT LIMITATION
A website cannot replace Chrome's browser engine or embed every site in its own tab. Chrome controls website tabs, downloads, login, and security. Downloads are handled by ChromeOS.

HOW TO USE IT
1. Unzip the folder.
2. Upload the four files (index.html, manifest.webmanifest, service-worker.js, icon.svg) to a static HTTPS host. Example: GitHub Pages, Cloudflare Pages, or another static host.
3. Open the resulting HTTPS URL in Chrome on the Chromebook.
4. Use Chrome's install option (often an install icon in the address bar, or menu > Install page as app / Create shortcut). Exact wording depends on ChromeOS version.
5. Launch Goggle Chrominium from the launcher or pin it to the shelf.

No Node.js is needed on the Chromebook. Hosting may be configured from another computer. Some hosts may ask you to sign in.

LOCAL PREVIEW
Opening index.html directly will let you try the interface and links, but installation and service-worker caching require HTTPS or localhost. Bookmarks are stored in that browser profile.

FILES
- index.html: interface and features
- manifest.webmanifest: PWA install metadata
- service-worker.js: app-shell caching
- icon.svg: app icon
