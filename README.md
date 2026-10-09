# Closet Log

My wardrobe as an iPhone home-screen app: a photo of every piece of clothing, sorted by section and type, with outfits, wear tracking, laundry, wishlist, stats and my size profile.

Everything is stored on the phone itself (photos in IndexedDB, the list in localStorage). Nothing is uploaded anywhere.

## Put it online (GitHub Pages)

1. On GitHub, create a new repository named **Closet-Log** (Public, no README).
2. On the empty repo page, click **uploading an existing file** and drag in all the files from this zip:
   `index.html`, `manifest.json`, `sw.js`, `icon-180.png`, `icon-192.png`, `icon-512.png`, `README.md`.
   They must sit directly in the repo, not inside a folder.
3. Click **Commit changes**.
4. Go to **Settings → Pages**. Under "Build and deployment", set **Source: Deploy from a branch**, **Branch: main**, folder **/ (root)**, then **Save**.
5. Wait a few minutes until the **Actions** tab shows a green ✓. The app is at:
   **https://prath-sec.github.io/Closet-Log/**

## Install on iPhone

1. Open the link in **Safari**.
2. Tap **Share → Add to Home Screen → Add**.
3. Open Closet Log from the home screen icon (not from Safari), so it runs full screen and keeps its own storage.

## Back up regularly

Data lives only on the phone. If Safari website data is cleared, or the app is removed from the home screen, it's gone.

- **Stats → Backup & restore → Save backup** opens the share sheet. Choose **Save to Files** and pick iCloud Drive or Google Drive.
- To restore: **Restore backup** and pick the `.json` file.

A backup once a week, or after adding many photos, is plenty.

## Updating the app later

Upload the new `index.html` over the old one (Add file → Upload files). Then open `sw.js`, change `closet-log-v1` to `closet-log-v2` (v3, and so on) and commit, so the phone picks up the new version. Close and reopen the app once.
