# Locator Color Lab — Android build

This repository wraps the standalone HTML app in a native Android WebView using Capacitor.

## Build an APK with GitHub Actions

1. Create a **new GitHub repository** named `locator-color-lab`.
2. Upload the contents of this folder to the repository root (make sure `.github/workflows/android-apk.yml` is included).
3. Open the repository's **Actions** tab.
4. Select **Build Android APK** and press **Run workflow**, or push a commit to `main`.
5. Wait for the workflow to finish successfully.
6. Open the completed workflow run and download the artifact named `locator-color-lab-debug-apk`.
7. Extract the ZIP artifact; install `app-debug.apk` on your Android phone.

## App details

- App name: Locator Color Lab
- Android application ID: `com.amory.locatorcolorlab`
- Build type: Debug APK (installable for testing)
- Web assets: `www/index.html` (font is embedded in the HTML)

## Notes

- This workflow creates the native Android project during CI, so generated Android/Gradle files do not need to be uploaded.
- The username lookup needs an internet connection. UUID-only calculation works offline.
- This is a debug APK for personal testing, not a Play Store release build.
