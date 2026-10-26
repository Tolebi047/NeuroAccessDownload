# NeuroAccess Android download page

A small static landing page for sharing the NeuroAccess Android APK. The page supports Kazakh, Russian, and English. iPhone distribution is intentionally postponed until the Android version is complete.

## Preview locally

Open `index.html` in a browser. The page has no build step. The APK download button stays disabled until `downloads/NeuroAccess-Android.apk` exists and is served by the site.

## Add the APK

Copy the finished APK to `downloads/NeuroAccess-Android.apk`. The page checks for that file and automatically enables the Android download link.

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
