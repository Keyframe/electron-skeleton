## Electron + React

`npx create-react-app electron-app`
`cd electron-app`
`npm install --save electron electron-builder wait-on concurrently`
`npm install --save electron-is-dev`
`cd public`
`touch main.js (check public/main.js)`
`cd ..`
`vi package.json`
add:
`"main": "public/electron.js"`
and
`"electron-dev": "concurrently \"BROWSER=none npm run start\" \"wait-on http://localhost:3000 && electron .\""`

`npm install`
`npm run electron-dev`
