# SPIDER SYSTEM 0.6 — Android Native

Android project adapted from the user's SPIDER SYSTEM 0.5 HTML prototype.

## What this build includes
- CameraX camera preview using Android's camera pipeline.
- Android SpeechRecognizer for Spanish voice commands.
- Android TextToSpeech for KAREN.
- Android location services with Google Maps handoff.
- Existing Homecoming-inspired HUD, subtitles and voice command logic.
- GitHub Actions workflow to compile a debug APK in the cloud (no Android Studio or laptop required).

## Build the APK from a phone using GitHub Actions
1. Create a repository on GitHub (a private repository is fine).
2. Upload the file `spider-system-0.6-android-project.zip` to the repository's root.
3. Create a file at `.github/workflows/build-apk.yml` and paste the contents of the included `build-apk.yml` file.
4. Commit the changes. GitHub Actions will start automatically. You can also open the **Actions** tab and run **Build SPIDER SYSTEM APK** using **Run workflow**.
5. Open the completed workflow run, scroll to **Artifacts**, and download `SPIDER-SYSTEM-0.6-debug-APK`.
6. Extract the downloaded artifact ZIP on Android and install `app-debug.apk`. Android may ask you to allow installs from the browser/file manager you used.

The workflow uses GitHub-hosted build machines. You do not need Android Studio, a PC, or a local Android SDK.

## Important limits
- This is a debug APK, not a Play Store release build.
- The native camera preview, speech recognition, TTS and GPS are integrated, but this project has not yet been tested on the user's physical phone.
- The camera preview appears behind the HUD inside the visor area; device-specific camera behavior still needs testing.
- Live HUD transmission to a physical mask/device is not included yet. It will need a network streaming feature and KAREN's explicit spoken confirmation before transmission.
- Real AI and facial recognition are not implemented.
