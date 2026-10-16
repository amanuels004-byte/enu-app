# Enu — Flutter Android starter

Enu is a Christian music and worship companion prototype built with Flutter.

## Included now
- Purple/cream Material 3 interface
- Import and play audio files stored on your phone
- Local favorites and recently played tracks
- Remove imported tracks from Enu's list (does not delete the original file)
- Offline sample faith conversation
- Local chat history saved on the device, with a clear-chat option
- Speech-to-text input and text-to-speech for replies (availability depends on Android speech services)
- Local profile name
- Mini-player with play/pause and stop controls

## Important limitations
- **This is not yet a production APK.** It is the Flutter source project.
- Faith chat currently uses built-in offline sample responses. It is **not a connected AI model**.
- The profile is a local profile, not a real login/account system.
- Music is not bundled. Import audio you own or are allowed to use.
- No cloud backup or cross-device sync is configured.
- I could not compile or run the Android build in this environment because the Flutter SDK is not installed here.

## Build on a computer with Flutter installed
1. Install Flutter and Android Studio, including the Android SDK.
2. Open a terminal in this project folder.
3. Run:
   ```bash
   flutter doctor
   flutter pub get
   flutter run
   ```
4. To create a release APK:
   ```bash
   flutter build apk --release
   ```
   The APK should be created at `build/app/outputs/flutter-apk/app-release.apk`.

## Dependencies
See `pubspec.yaml`. Flutter will fetch the packages with `flutter pub get`.

## Next production steps
1. Add Android application ID, app icon, and permission review in generated Android project files.
2. Connect a secure backend for real AI conversations (never put a private API key in the mobile app).
3. Add real authentication and secure cloud storage only after choosing a backend.
4. Test audio persistence, voice input, accessibility, and Android versions on a real phone.
5. Review music licensing and privacy disclosures before public release.
