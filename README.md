# ScreenPing — Android Unlock Screen Time Notifier

Tracks active screen time from each phone unlock event (`ACTION_USER_PRESENT`), sends a high-priority notification every **1 minute(s)** (`"You have been using phone for 1 minute"`, `"You have been using phone for 2 minutes"`, `"You have been using phone for 3 minutes"`), and records multiple sessions across the day.

## Build & Install

1. Open this folder in **Android Studio** (Hedgehog / Koala / Ladybug or newer).
2. Connect an Android device (Android 8.0+ / API 26+) with USB Debugging enabled, or launch an emulator.
3. Click **Run 'app'** or run via terminal:
   ```bash
   ./gradlew assembleDebug
   adb install -r app/build/outputs/apk/debug/app-debug.apk
   ```
4. On first launch (Android 13+), tap **Allow** on the notification permission prompt and tap **Allow Unrestricted Background Battery Usage** so the OS never suspends the unlock monitor.
