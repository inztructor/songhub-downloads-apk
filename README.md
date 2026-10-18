# SongHub Downloads APK

This repository wraps the live Blogger website:
https://songhubdownloads.blogspot.com/

## Build without installing tools on your computer

1. Create a GitHub repository (for example, `songhub-downloads-apk`).
2. Upload the contents of this folder, preserving the `.github/workflows/` path.
3. Commit the files to the `main` branch.
4. Open the repository's **Actions** tab.
5. Select **Build SongHub Downloads APK** and choose **Run workflow**.
6. When the run succeeds, download the `SongHub-Downloads-APK` artifact.
7. Extract the ZIP to get `app-debug.apk`.

The GitHub Actions runner installs Node.js, Java, and Android SDK in the cloud.
You do not need to install Node.js, Git, or Android Studio on your computer.

## Notes

- This is a debug APK for testing and direct installation, not a signed Play Store release.
- The app loads the live Blogger website and therefore needs internet access.
- Test navigation and all file-download links on an Android phone. Some external downloads may require additional native handling.
- The workflow retains the APK artifact for 14 days.
