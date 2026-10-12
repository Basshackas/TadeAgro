# TadeAgro

Farm investment tracker for Tadesse Farms (banana, tomato and pepper farms, each with batches).

## Put it online with GitHub Pages
1. On github.com create a new repository (for example `tadeagro`). A free account needs it to be public. The app is encrypted, so its code and data are unreadable without your access code.
2. Upload every file from this folder (Add file > Upload files). Include `index.html`, `sw.js`, the images, `manifest.webmanifest`, `robots.txt` and `.nojekyll`.
3. Settings > Pages > Deploy from a branch > `main` / `(root)` > Save.
4. After a minute the app is at `https://YOUR-USERNAME.github.io/REPOSITORY-NAME/`.
5. Open it on your phone, enter the access code, then Settings > Install on your phone.

## Works offline
After the first visit the app opens and works with no internet: adding and editing entries, Excel import and export, receipt photos and the PDF statement all run on the phone. Only fonts and Google Drive backup need a connection.

## Google Drive backup (optional)
Settings > Google Drive backup keeps a copy of your data in your own Drive. It updates by itself whenever the app is open and online, and you can also tap Back up now or Restore. A web app cannot run in the background when it is closed, so the backup happens the next time you open it with internet.

One-time setup (about 5 minutes):
1. Go to console.cloud.google.com and create a project.
2. Enable the Google Drive API.
3. OAuth consent screen: choose External and add each partner's Google account as a test user.
4. Credentials > Create credentials > OAuth client ID > Web application. Under Authorized JavaScript origins add your site address, for example `https://YOUR-USERNAME.github.io` (no path at the end).
5. Copy the client ID, open Settings > Google Drive backup in the app and paste it.

The app asks only for the narrow `drive.file` permission, so it can see only the one backup file it creates. Each partner connects their own Google account and gets their own backup.

## Access code
Share the code only with people you trust. To change it, use the separate private `change-access-code.html` tool (never upload that file) and replace `index.html` on GitHub with the file it makes. Everyone then needs the new code.

## Your data
- Each phone keeps its own data in its browser. Use Settings > Save backup file and Load backup file to move or share data between phones.
- To bring in data from the older Claude-hosted version, save a backup there and load it here.
- The PIN lock (Settings > Security) is an extra lock for one phone.
