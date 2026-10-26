# NeuroAccess Android download page

A small static landing page for sharing the NeuroAccess Android APK. The page supports Kazakh, Russian, and English. iPhone distribution is intentionally postponed until the Android version is complete.

## Preview locally

Open `index.html` in a browser. The page has no build step. The Android download button points to the latest GitHub Release asset.

## Upload the APK as a GitHub Release asset

The current APK is about 118 MB, larger than GitHub's 100 MB regular repository file limit. Keep it out of the Pages source and upload `release-assets/NeuroAccess-Android.apk` as an asset on a GitHub Release. Release assets can be up to 2 GiB each. Use the asset name `NeuroAccess-Android.apk`; the page links to the latest release download.

## Runtime requirement

The current demo recognition API still runs on the developer laptop. Users must start that server, connect their Android phone to the same Wi-Fi or hotspot, and enter the server address in the app settings.

## Publish for free with GitHub Pages

Create a **public** GitHub repository for this site. GitHub Pages is available for public repositories on GitHub Free. Then, from this directory, run:

```powershell
git init -b main
git add .
git commit -m "Create NeuroAccess Android download site"
git remote add origin https://github.com/YOUR-USERNAME/NeuroAccessDownload.git
git push -u origin main
```

In GitHub, open **Settings → Pages** and choose **GitHub Actions** as the build and deployment source. The included workflow publishes the site at `https://YOUR-USERNAME.github.io/NeuroAccessDownload/`.
