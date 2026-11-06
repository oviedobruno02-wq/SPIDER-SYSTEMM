SPIDER SYSTEMM 0.6 — Android project starter

This package restores the supplied 0.5 HUD as the app's initial screen and wraps it
in an Android WebView hosted on a secure local appassets origin. The native wrapper
requests Android camera, microphone and location permissions.

Included baseline features from the supplied HTML:
- Camera preview and HUD overlay
- Immersive visor / fullscreen mode
- KAREN text-to-speech (device/browser engine dependent)
- Voice command recognition (WebView engine dependent)
- GPS / Google Maps link
- Subtitles and system diagnostics
- Original KAREN spider icon

Not included yet:
- AI backend / online assistant
- Face recognition
- Mask streaming (intentionally postponed; no Emitir control)
- Guaranteed native SpeechRecognizer integration; that is a later implementation step

Build:
1. Upload spider-system-0.6-android-project.zip to the root of the GitHub repository.
2. Add .github/workflows/build-apk.yml to the repository (provided separately).
3. Open GitHub > Actions > Build SPIDER SYSTEM APK > Run workflow.
4. When the run succeeds, download the artifact named SPIDER-SYSTEM-0.6-debug-APK.
5. Install app-debug.apk on the Android device.

The project has not been compiled in this environment. A successful GitHub Actions
build is required before calling the APK installable.
