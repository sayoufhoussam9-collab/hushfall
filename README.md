# Hushfall

A free sleep sounds app for phones. It has no ads, no accounts and no locked sounds.

All 19 sounds are generated live in the browser with the Web Audio API. There are no audio files, so there is nothing to license or download.

## Features

- **Sounds:** rain, downpour, thunder, ocean, stream, wind, campfire, crickets, owl, night train, white, pink and brown noise, fan, wind chimes, deep drone, heartbeat, cat purr and old clock
- **Mixing:** play any number of sounds at once, each with its own volume
- **Mixes:** 8 ready-made mixes, and you can save your own on your device
- **Sleep timer:** 15 minutes to 4 hours, with a 30 second, 2 minute or 5 minute fade-out
- **Dim screen:** a black screen that shows only a faint clock
- **Installable and offline:** includes a web app manifest and a service worker

## Run it

This is a static site with no build step. Serve the folder over HTTPS (for example with GitHub Pages) and open `index.html`. On a phone, use **Add to Home Screen** to install it. After the first visit it works offline.

To try it on your computer:

```
npx serve .
```

## Files

| File | Purpose |
| --- | --- |
| `index.html` | The whole app: UI, sound engine and timer |
| `manifest.webmanifest` | App name, colors and icons for installing |
| `sw.js` | Service worker that caches the app for offline use |
| `icon.svg`, `icon-192.png`, `icon-512.png` | App icons |
