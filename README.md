# Swift Wave – Android app

Wraps the Swift Wave web app (`app/src/main/assets/index.html`) in a native Android WebView.
Camera (selfie) and document upload work through Android permissions.

## Option A – Build online with GitHub (nothing to install)
1. Create a new repository on github.com and upload the contents of this folder (keep the `.github` folder).
2. Open the **Actions** tab. "Build Swift Wave APK" runs automatically (or press **Run workflow**).
3. When it finishes (about 5 minutes), open the run and download **SwiftWave-apk** under *Artifacts*.
4. Unzip it, copy `app-debug.apk` to your phone and open it. Allow "Install unknown apps" when asked.

## Option B – Build with Android Studio
1. Open this folder in Android Studio and let Gradle sync.
2. **Build → Build App Bundle(s) / APK(s) → Build APK(s)**, or connect your phone and press **Run**.

## Updating the app
Replace `app/src/main/assets/index.html` with the latest web version and rebuild.

## Notes
- Debug APKs are signed with a debug key: fine for testing and demos, not for the Play Store.
- Live chat uses the built-in assistant (the Claude-powered chat only runs inside Claude).
- Fonts load from Google Fonts when online; system fonts are used offline.
