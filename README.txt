NEXTBALL OFFLINE - Android Studio project

What this build does:
- Bundles the supplied single-file game inside the app.
- Opens it from local Android assets (no website hosting required).
- Locks the app to landscape and immersive full-screen mode.
- Removes remote Firebase script downloads and the Google Fonts stylesheet.
- Does not request Android INTERNET permission.

Important limitations:
- Firebase-dependent online features (account/login, cloud saves, online rooms/multiplayer)
  cannot work offline and are intentionally unavailable in this offline package.
- This project is Android source code, not a signed APK.
- To build: open this folder in Android Studio, allow Gradle sync, then Build > Build Bundle(s) / APK(s) > Build APK(s).

Automatic APK build with GitHub Actions:
1. Upload the contents of this project folder to your GitHub repository (main branch).
2. Open the repository's Actions tab.
3. Select "Build NEXTBALL Offline APK" and choose "Run workflow" if it has not started automatically.
4. When the workflow completes, open the run and download the "NEXTBALL-Offline-APK" artifact.
5. Extract the downloaded artifact ZIP to get app-debug.apk, then install it on your Android phone.
