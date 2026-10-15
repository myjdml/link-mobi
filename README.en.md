# LinkMobi

[简体中文](./README.md) | **English**

An unofficial, simplified Android edition adapted from the discontinued Mobi Fitness app, with no login required. AI tools were used throughout the adaptation and packaging. This repository shares APKs without source code; updated versions may follow.

Original app: **Mobi Fitness 4.5.16.1**. LinkMobi uses its own version numbering.

## Download

**[Download LinkMobi-0.0.1.apk](./LinkMobi-0.0.1.apk?raw=true)**

Version `0.0.1` · Android 8.0 or later · App language: Simplified Chinese

SHA-256:

```text
16432beff4d27a5de00a291655b599d478f0c669cbcf65570e187572b7a11e9a
```

## Features

- Bluetooth equipment connection and free workouts without login.
- Local profile, workout history, and JSON export.
- Phone and tablet layouts with portrait and landscape support.
- Selectable elliptical metrics and smart resistance, depending on equipment support.

Original cloud courses, online races, social features, cloud history, and firmware downloads are not restored. Paid content is not unlocked. Emulator checks have been completed; physical equipment and devices using 16 KB memory pages still need testing.

## Screenshots

Captured on an Android emulator with simulated workout data.

| Home | Free workout | Workout history |
| :---: | :---: | :---: |
| <img src="./assets/screenshots/home.png" alt="LinkMobi home screen" width="240"> | <img src="./assets/screenshots/workout.png" alt="LinkMobi free workout" width="240"> | <img src="./assets/screenshots/history.png" alt="LinkMobi workout history" width="240"> |

Landscape workout:

<img src="./assets/screenshots/workout-landscape.png" alt="LinkMobi landscape workout" width="760">

## Installation and use

1. Download and open the APK on Android, allowing installation when prompted.
2. Open the app, update your profile, turn on Bluetooth, and grant permissions in device management to connect your equipment.
3. Start a free workout, then view local records or export JSON for backup.

Install over an existing offline edition from this project. The official app uses a different signing certificate: back up any data you can preserve, then uninstall it before installing this APK. Uninstalling deletes the original app's local data.

## Release history

`0.0.1` · 2026-10-15: First public LinkMobi release with consistent app and APK naming. Future versions start at `0.0.2`.

## License

This project is licensed under the [Apache License 2.0](./LICENSE).
