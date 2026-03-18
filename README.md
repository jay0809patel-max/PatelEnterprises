# Scripts Launcher PWA

A clean, installable Progressive Web App to launch your web app scripts and tools from your phone's home screen — on both Android and iOS.

---

## Files
- `index.html` — The full app
- `manifest.json` — PWA metadata (name, icons, display mode)
- `sw.js` — Service worker (enables offline use + installability)
- `icon-192.png` / `icon-512.png` — App icons (you need to add these)

---

## Deploy in 5 minutes (free) — GitHub Pages

1. Create a free account at https://github.com
2. Create a new **public** repository (e.g. `my-scripts`)
3. Upload all files in this folder
4. Go to **Settings → Pages → Source → main branch / root**
5. Your app will be live at: `https://yourusername.github.io/my-scripts`

---

## Install on Android
1. Open the URL in **Chrome**
2. Tap the **⋮ menu → "Add to Home screen"**
3. Done — it appears as an app icon!

## Install on iOS
1. Open the URL in **Safari** (must be Safari)
2. Tap the **Share button (□↑) → "Add to Home Screen"**
3. Done!

---

## Add Your App Icons
You need two PNG icon files:
- `icon-192.png` (192×192 px)
- `icon-512.png` (512×512 px)

You can make them at: https://www.canva.com or https://favicon.io

---

## Customise
All your scripts are stored in the browser's `localStorage` — no server needed.
Open the app → tap **+** → add your real Google Apps Script URLs.

To pre-load your scripts instead of the sample data, edit the `defaultScripts` array in `index.html`:

```js
const defaultScripts = [
  { id: 1, name: 'My Tool', url: 'https://script.google.com/…', desc: 'What it does', category: 'Reports', icon: '📊' },
  // add more…
];
```
