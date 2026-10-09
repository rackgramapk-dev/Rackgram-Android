# Rackgram Android APK build project

This repository contains the Android APK build setup for the Rackgram web app. The app source is bundled from the existing Rackgram build flow and prepared for Capacitor Android builds.

## Structure

- `index.html` — app shell and main UI logic
- `package.json` — Capacitor + Supabase + LiveKit dependencies
- `capacitor.config.json` — Android app config
- `.github/workflows/build-apk.yml` — GitHub Actions APK build pipeline
- `android-native/` — Android Java notification and lock-screen handling
- `supabase/` — database and edge-function SQL for calls and notifications

## Build

Push to `main` and run the GitHub Actions workflow `Build APK`.

The generated artifact will be created at:

`android/app/build/outputs/apk/debug/app-debug.apk`
