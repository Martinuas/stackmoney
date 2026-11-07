# Stack Money

A simple, private budgeting tool. Track bank, debt and savings balances, log spending by hand, and keep one goal in front of you all month.

**Privacy:** there is no server and no account. Everything is stored in the user's own browser (localStorage) and is never uploaded. The site contains no analytics, ads or third-party scripts.

## Publish it (GitHub Pages, free)

1. Create a GitHub account, then a new **public** repository (for example `stackmoney`).
2. Click **Add file → Upload files**, drag in everything in this folder (including `.nojekyll`), and commit.
3. Go to **Settings → Pages**. Under "Build and deployment" choose **Deploy from a branch**, branch `main`, folder `/ (root)`, and Save.
4. After a minute your site is live at `https://YOUR-USERNAME.github.io/stackmoney/`. HTTPS is automatic.

Netlify or Cloudflare Pages also work: connect the repository, leave the build command empty, and set the publish directory to the repository root.

## Update it later

Edit `index.html` on GitHub (pencil icon) and commit. If you want installed copies to refresh right away, also change `CACHE = "stackmoney-v1"` in `sw.js` to `v2`, `v3` and so on.

## Use it on a phone

- **iPhone (Safari):** Share → Add to Home Screen.
- **Android (Chrome):** menu → Install app / Add to Home screen.

Installing is optional. It just makes the tool open like an app and work offline. Nothing is downloaded beyond the page itself.

## What is in this folder

| File | Purpose |
|---|---|
| `index.html` | The whole app |
| `manifest.webmanifest`, `icon*.png/svg` | Make it installable on phones |
| `sw.js` | Lets it open offline |
| `.nojekyll` | Tells GitHub Pages to serve files as-is |

## Good to know

- Data lives per browser per device. Phone and computer do not sync. The "Copy backup" and "Restore" buttons move data between them.
- Clearing browser data erases the budget. Safari may also clear data for sites that are not opened for a long stretch unless the app is added to the Home Screen, so remind users to back up.
- Please keep real account numbers and passwords out of the tool. Balances and amounts are all it needs.
