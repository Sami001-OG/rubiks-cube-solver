# CUBE.SYS: 3D Rubik's Cube Solver

Single-file web app (three.js + [cubejs](https://github.com/ldez/cubejs) Kociemba two-phase solver, all inlined). No build step, works offline.

- **Solved cube**: scramble it yourself, then STEP or SOLVE ALL.
- **Custom cube**: paint every sticker to match your real cube; the cube is validated, then solved.

## Run locally
Open `index.html` in a browser, or serve it: `python3 -m http.server 8000` and visit http://localhost:8000.

## Install as an app (PWA)
Serve over HTTPS (GitHub Pages) or localhost, then use "Install app" in Chrome/Edge or "Add to Home Screen" on mobile.

## Desktop app (optional)
```
npm init -y && npm i -D electron
# main.js: const {app,BrowserWindow}=require('electron');app.whenReady().then(()=>new BrowserWindow({width:1100,height:800}).loadFile('index.html'))
npx electron .
```
