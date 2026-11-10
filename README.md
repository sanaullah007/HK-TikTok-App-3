# HK — TikTok-style short video Android app

This is an **original HK-branded short-video prototype**, not TikTok itself. Built with React Native + Expo.

## Features
- Full-screen vertical video feed; swipe up/down; autoplay, pause/play
- For You / Following feed, like, comment, follow, save, share
- Search/discover posts and creators
- Device video picker, video posting in the local session
- Profile, own videos, saved videos, inbox placeholder

**Important:** Authentication, cloud video hosting, persistent posts/comments, public interactions, notifications, moderation, and production-grade storage are **not implemented**. This is a runnable demo, not a production-ready social network. Sample videos load from public URLs and require internet.

## Build an APK using GitHub Actions
1. Create a new GitHub repository, for example `HK-App`.
2. Upload **all files and folders inside this project** to the repository root. Preserve `.github/workflows/android-apk.yml`.
3. Open the GitHub repository > **Actions** > **Build HK Android APK** > **Run workflow** (or push to `main`).
4. When the workflow finishes successfully, click the workflow run > **Artifacts** > **HK-Android-APK**.
5. Download and unzip the artifact. Install `app-debug.apk` on an Android phone with permission to install apps from the source.

## Local preview
```bash
npm install
npx expo start
```

Use Expo Go (SDK-compatible version) on a phone or build with Android Studio. Debug APK is for testing only. Production release requires signing, security reviews, backend and store compliance.
