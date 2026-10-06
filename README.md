# TadeAgro

Farm investment tracker for Tadesse Farms (banana, tomato and pepper farms, with batches).

## Put it online with GitHub Pages
1. On github.com create a new repository (for example `tadeagro`). A free account needs it to be public. The app itself is encrypted, so the code and data inside are unreadable without your access code.
2. Upload every file from this folder to the repository (Add file > Upload files). Include `index.html`, the images, `manifest.webmanifest`, `robots.txt` and `.nojekyll`.
3. Open Settings > Pages. Under Build and deployment choose Deploy from a branch, branch `main`, folder `/ (root)`, then Save.
4. After a minute your app is at `https://YOUR-USERNAME.github.io/REPOSITORY-NAME/`.
5. Open it on your phone, enter the access code, and use Add to Home screen to install it as TadeAgro.

## Access code
The app asks for an access code on the first visit on each phone. Share the code only with people you trust. To change it, use the private `change-access-code.html` tool that came separately (never upload that file) and replace `index.html` on GitHub with the new one it makes. Everyone then needs the new code.

## Data
- Each phone keeps its own data in its browser. Use Save backup file and Load backup file on the Overview tab to move or share data between phones.
- The PIN lock (Overview) is an extra lock for one phone.
- To bring over data from the Claude-hosted version, save a backup there and load it here.
