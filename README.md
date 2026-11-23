# Ratan Bhaban Android app

This is an Android Studio project that wraps the live Ratan Bhaban website:
https://biplobbiswash.github.io/Ratan-Bhaban/

## Build the APK
1. Install Android Studio on a computer.
2. Extract this ZIP.
3. In Android Studio, choose **Open** and select the `RatanBhabanAndroid` folder.
4. Allow Gradle sync and install the suggested Android SDK (API 35).
5. Select **Build > Build Bundle(s) / APK(s) > Build APK(s)**.
6. When the build finishes, choose **locate**. The APK is usually at:
   `app/build/outputs/apk/debug/app-debug.apk`

## Included
- App title: Ratan Bhaban
- Blue/white RT-style launcher icon placeholder can be added in Android Studio
- WebView with JavaScript and local storage enabled
- Android back navigation
- Progress indicator
- JSON restore file picker support
- External links, including Google sign-in, open in the system browser

## Important notes
- This app loads the live website, so an internet connection is required.
- Your website says its records are stored in the browser on the device. WebView storage is enabled, but data saved in the Chrome browser and data saved inside this app are separate.
- Google Drive sign-in may not work inside embedded WebViews because Google restricts some embedded-browser sign-in flows. The app opens external pages in the system browser; if the Drive connection flow does not return to the app, use the website's **Backup JSON / Restore file** option.
- This is a debug-build project. For Play Store or wider distribution, create a signed release APK in Android Studio and configure a production signing key.


## Build APK automatically with GitHub (no Android Studio needed)
1. Create a GitHub repository, for example `Ratan-Bhaban-Android`.
2. Upload all files and folders from this project, including the hidden `.github` folder.
3. Open the repository's **Actions** tab.
4. Select **Build Ratan Bhaban APK** and click **Run workflow** (or wait for the push build).
5. Open the completed workflow run and download the `Ratan-Bhaban-APK` artifact.
6. Extract the downloaded artifact ZIP; it contains `app-debug.apk`.

The workflow builds the APK in GitHub's hosted runner and stores it as a downloadable Actions artifact.
