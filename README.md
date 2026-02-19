# Pull Strength BLE App

[![Flutter](https://img.shields.io/badge/Flutter-02569B?logo=flutter&logoColor=white)](https://flutter.dev)
![Platform](https://img.shields.io/badge/Platform-Android-3DDC84?logo=android&logoColor=white)
![BLE](https://img.shields.io/badge/BLE-supported-1E88E5)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

A Flutter app for Android that connects to a BLE crane scale (WeiHeng WH-C06 compatible), decodes live readings, and tracks left/right pull test history over time.

## Features

- Scan for nearby BLE devices and connect to your scale.
- Decode advertisement payloads into live weight readings.
- View a real-time chart of incoming measurements.
- Run left/right pull tests and store max values.
- Persist test history locally on device.
- Visualize progression with left/right trend lines.

## Screenshots

### Overview

<img src="docs/screenshots/overview.png" alt="Overview Screen" width="256" />

### Device Connection

<img src="docs/screenshots/connection.png" alt="Connection Screen" width="256" />

### Live Reading

<img src="docs/screenshots/live-reading.png" alt="Live Reading Screen" width="256" />

### Pull Test

<img src="docs/screenshots/pull-test.png" alt="Pull Test Screen" width="256" />


## Tech Stack

- Flutter (Material 3)
- `flutter_blue_plus` for BLE scanning and advertisement handling
- `fl_chart` for live/progression charts
- `shared_preferences` for local history persistence


## Getting Started

### Prerequisites

- Flutter SDK installed
- Android Studio / Android SDK
- WeiHeng WH-C06 Bluetooth Crane Scale
- A physical Android device with Bluetooth support (recommended for BLE)

### Install dependencies

```bash
flutter pub get
```

### Run on Android

```bash
flutter run
```

## Usage

1. Open the app and go to the connection setup.
2. Start scanning and select your BLE scale.
3. Open the live page to monitor incoming readings.
4. Perform left/right tests and store results.
5. Review your progression chart on the overview screen.

## Notes

- BLE behavior can vary by Android version and device vendor.
- For best results, keep the scale close to the phone and minimize BLE interference.

## Future Improvements

- Export test history (CSV/JSON)
- Workouts/Guided Sessions with zones in force charts and timers to guide the workout
- Session tagging / notes
- Multi-device profile support


