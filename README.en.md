# LinkMobi

[简体中文](./README.md) | **English**

An unofficial, simplified Android edition adapted from the discontinued Mobi Fitness app, with no login required. AI tools were used throughout the adaptation and packaging. This repository shares APKs without source code; updated versions may follow.

Original app: **Mobi Fitness 4.5.16.1**. LinkMobi uses its own version numbering.

## Download

**[Download LinkMobi-0.0.2.apk](./LinkMobi-0.0.2.apk?raw=true)**

Version `0.0.2` · About 92.7 MiB · Android 8.0 or later · App language: Simplified Chinese

SHA-256:

```text
b0635c295b28c7d3b1a963a6170247b726d0208818224e3ae2fdcb7a1a372386
```

## New in 0.0.2: workout overlay

View workout data while using other apps, and adjust resistance, speed, or incline when supported by your equipment.

- **Uses little screen space:** appears only at the top center, with a width that follows its content. The translucent black capsule has green accents and fully rounded ends. It sits directly below the status bar or cutout safe area without an extra top gap. On Android 11 or later, it moves higher when a fullscreen app hides the status bar. It suits landscape use and also supports portrait, phones, and tablets.
- **Key metrics stay visible:** the collapsed single row shows duration, distance, heart rate, and an equipment metric. Treadmills show speed, equipment with resistance feedback shows the resistance level, and other equipment shows calories. Missing values appear as “—”.
- **Expand for controls:** tap the bar to reveal supported resistance, speed, and incline controls, plus return, collapse, and dismiss actions. Smart resistance mode hides manual resistance buttons. Disconnection marks the data as no longer updating and disables controls.
- **Appears automatically:** leave the workout screen during an active session to show the overlay; return to hide it, or finish the workout to remove it. It remains available while paused. Each session starts collapsed, and dismissing applies only to that session. Pause, resume, and finish remain on the workout screen.
- **One simple setting:** the overlay is off by default and has a single enable switch. Grant Android’s “Display over other apps” permission when prompted. Workouts still work without this permission.

## Features

- Bluetooth equipment connection and free workouts without login.
- Local profile, workout history, and JSON export.
- Phone and tablet layouts with portrait and landscape support.
- Selectable elliptical metrics and smart resistance, depending on equipment support.
- A top workout overlay for viewing data across apps and adjusting supported equipment controls.

Original cloud courses, online races, social features, cloud history, and firmware downloads are not restored. Paid content is not unlocked. Emulator checks have been completed; physical equipment and devices using 16 KB memory pages still need testing.

## Screenshots

Captured in version 0.0.2 on an Android emulator with simulated workout data.

Top overlay, collapsed in landscape:

<img src="./assets/screenshots/overlay-collapsed.png" alt="LinkMobi 0.0.2 collapsed top overlay showing duration, distance, heart rate, and resistance" width="900">

Top overlay, expanded in landscape with resistance controls:

<img src="./assets/screenshots/overlay-expanded.png" alt="LinkMobi 0.0.2 expanded top overlay with resistance decrease and increase buttons" width="900">

| Home | Free workout | Workout history |
| :---: | :---: | :---: |
| <img src="./assets/screenshots/home.png" alt="LinkMobi home screen" width="240"> | <img src="./assets/screenshots/workout.png" alt="LinkMobi free workout" width="240"> | <img src="./assets/screenshots/history.png" alt="LinkMobi workout history" width="240"> |

Landscape workout:

<img src="./assets/screenshots/workout-landscape.png" alt="LinkMobi landscape workout" width="760">

## Installation and use

1. Download and open the APK on Android, allowing installation when prompted.
2. Open the app, update your profile, turn on Bluetooth, and grant permissions in device management to connect your equipment.
3. Start a free workout, then view local records or export JSON for backup.
4. To view workout data across apps, enable “训练悬浮窗” (workout overlay) in Settings or through the workout screen’s overlay entry, grant the system overlay permission, then leave the workout screen during a session.

Install over an existing offline edition from this project. Upgrading from 0.0.1 has been verified to preserve the profile, workout history, and remembered equipment. The official app uses a different signing certificate: back up any data you can preserve, then uninstall it before installing this APK. Uninstalling deletes the original app's local data.

Version 0.0.2 passed emulator checks for overlay permissions, background updates, collapse and expand, rotation, and simulated equipment controls, plus regression checks for four equipment types, record saving, and JSON export. APK signature and ZIP alignment checks passed. Resistance, speed, and incline control still require validation with physical equipment.

## Release history

- `0.0.2` rebuild · 2026-10-19: Moved the overlay higher by removing the extra top gap and following fullscreen status bar visibility on Android 11 or later. The version number is unchanged.
- `0.0.2` · 2026-10-18: Added the top workout overlay with data across apps, persistent heart rate, collapse and expand, and equipment controls. Introduced a green capsule sized to its content and a single enable setting. Updated screenshots and instructions, retaining the existing signing certificate for upgrades.
- `0.0.1` · 2026-10-15: First public LinkMobi release with consistent app and APK naming.

## License

This project is licensed under the [Apache License 2.0](./LICENSE).
