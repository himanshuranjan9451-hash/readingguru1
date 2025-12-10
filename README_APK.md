# Reading Guru - APK Build Instructions (One-click via GitHub Actions)

This repo is set up to automatically build an **Android debug APK** using **GitHub Actions** when you push the code to GitHub (branch `main` or `master`).

## How it works (quick)
1. Create a GitHub account (if you don't have one) and create a new repository named `reading_guru` (or any name).
2. Upload the contents of this folder to that repository (you can upload ZIP in GitHub web UI).
3. Push to branch `main` (or `master`). The GitHub Action will run and produce an artifact named `reading_guru_apk`.
4. After the workflow completes, go to the "Actions" tab in your GitHub repo, open the latest run, and download the artifact `reading_guru_apk` which contains `app-debug.apk`.
5. Transfer the APK to your Android phone and install (enable Install from Unknown Sources).

## Important notes
- The APK built is a **debug APK** (unsigned). It's fine for testing on Android devices. If you want a signed release APK, additional steps are needed (keystore and secrets).
- You do **not** need a laptop to do this — you can upload the ZIP via your phone's browser or GitHub mobile app and trigger the workflow. The build runs on GitHub servers.
- For consistent Indian-accent TTS, devices might still use device voices. To use Google Cloud TTS you'll need to add backend server or CI secrets (not included here).

## Steps to push from phone (easy)
1. Open GitHub (mobile browser) and create a new repo.
2. Use "Add file" -> "Upload files" and upload all files from this package (you may upload the ZIP and extract via GitHub web? If not possible, upload files directly).
3. Commit to `main`. Go to Actions tab and wait ~5–10 minutes for build.
4. Download artifact and install APK on phone.

If you want, I can also:
- Create the GitHub repo for you (you'll need to give me a GitHub access token — not recommended). 
- Or I can walk you step-by-step via phone screen instructions to upload and download the APK.
