# Offline Notes Lab

A small, installable, offline-first Progressive Web App (PWA) built with React, TypeScript, and Vite. Users can create notes, which are stored locally in the browser, and the app remains usable offline thanks to a service worker caching the application shell.

## Live demo
 https://smiggle001.github.io/offline-notes-lab

## Run locally
npm install
npm run dev

## Verify the build
npm run check
npm run build
npm run preview

## PWA test
1. Open the preview (or live) URL and let it load fully at least once while online, so the service worker registers.
2. Open browser DevTools → Application → Service Workers, and confirm the worker shows as activated.
3. Switch Network to Offline (DevTools → Network, or the checkbox in the Service Workers panel).
4. Reload the page — it should still load from cache.
5. Create a note while offline and refresh again — it should persist (notes are stored in localStorage, separately from the cached app shell).

## Environment
- Node.js version used: v24.20.0
- Package manager: npm
