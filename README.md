# Prospect Ops — Installable Android App (No Chrome "Add to Home Screen")

This project packages the Prospect Ops offline web app into a **real Android APK** using a simple **WebView** wrapper.
It loads: `file:///android_asset/index.html`

## Option A (Easiest): Build APK with GitHub (no PC build tools on your side)
1) Create a free GitHub account (if you don't have one).
2) Create a new repo and upload **all files** from this zip.
3) In GitHub, go to **Actions** → enable Actions if asked.
4) Click **Build Android APK** workflow → **Run workflow**.
5) When it finishes, download the artifact: **ProspectOps-debug-apk** → `app-debug.apk`
6) Copy the APK to your phone and install it (allow "Install unknown apps" once).

## Option B: Build in Android Studio (PC)
1) Install Android Studio
2) Open this folder as a project
3) Click **Build → Build APK(s)**
4) Install the generated `app-debug.apk` on your phone.

## Notes
- Data is stored inside the WebView using localStorage, like before.
- Backup/Restore works inside the app (downloads a JSON backup).
- If you want a Play Store version, you'll build an AAB + sign it (next step once this is stable).

## Included Web Pack
Embedded from: `Prospect_Ops_Upgrade_v2.zip`
