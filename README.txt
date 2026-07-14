DayZ Stash Tracker — Usage

How to run:

- Open index.html in your browser (double-click or use the Start-Process PowerShell command).

Basic usage:

- Add a stash using the form: provide a name, optional notes, and save.
- Each stash shows a live countdown and has a "Reset" control to restart its timer.
- Stashes are saved automatically in localStorage and will persist across reloads.

Notes:

- The app includes manifest.json and config.xml for installing as a PWA or packaging with Cordova.
- No server or installation is required — just open the index.html file.

That's it.

Run as a desktop app (Electron)

 - Prerequisites: install Node.js (includes `npm`).
 - From the project root, install dependencies and start the app:

```powershell
npm install
npm start
```

 - To create a Windows build (requires `electron-packager`):

```powershell
npm run package-win
```

Notes:

 - The packaging command uses `electron-packager` via `npx`; you can install it globally if preferred.
 - If you want a single EXE installer, consider `electron-builder` instead — I can scaffold that if you want.
