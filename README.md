# Grosvenor plant guide app

This folder is the BioCondition plant field guide set up as an offline web app for iPhone.

| File | What it is |
|---|---|
| index.html | The guide, with all photos built in (about 14 MB) |
| sw.js | Saves the guide on the phone so it works without signal |
| manifest.webmanifest | App name, icon and full-screen setting |
| icon-180.png, icon-192.png, icon-512.png | Home Screen icons |

## 1. Put it online (on a computer, about 5 minutes)

1. Sign in at github.com (a free account is fine).
2. Click **+** (top right), then **New repository**. Use a name that doesn't point to the client, for example `field-guide-g26`. Leave it **Public**, because free GitHub Pages needs a public repository. Click **Create repository**.
3. On the new repository page, click **uploading an existing file**. Drag in all 7 files from this folder (the files themselves, not the folder), then click **Commit changes**.
4. Go to **Settings**, then **Pages**. Under Source choose **Deploy from a branch**, set the branch to **main** and the folder to **/ (root)**, then click **Save**.
5. Wait 1 to 2 minutes and refresh. Your link appears at the top, for example `https://yourname.github.io/field-guide-g26/`.

## 2. Install it on the iPhone (with good signal)

1. Open the link in **Safari**. It must be Safari, not Chrome.
2. Tap **Share**, then **Add to Home Screen**, then **Add**.
3. **Open the app from the new Home Screen icon** and wait until the green line reads "Saved on this phone. Works without signal". The Home Screen app keeps its own offline copy, separate from Safari, which is why this step matters.
4. Turn on Airplane Mode, close the app and open it again to check that it works offline.

Tip: open it once with signal the day before each field trip.

## Updating or taking it down

- **To update the guide:** upload the new `index.html`, then edit `sw.js` and change `VERSION` (for example to `grosvenor-guide-v2`). Open the app once with signal to pick up the change.
- **To take it down:** in the repository go to **Settings**, then **Pages**, and unpublish it, or delete the repository.

The page is public to anyone who has the link. It asks search engines not to list it, but don't share the link more widely than needed.
