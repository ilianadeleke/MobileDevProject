# MobileDevProject

MobileDevProject is a Kotlin-based Android fitness and nutrition tracking application designed to help users monitor their daily calorie intake, log exercises, and stay on track with their health goals.

## Overview

The app combines food logging, exercise tracking, goal setting, notifications, and location-based features in one simple mobile dashboard. It allows users to:

- Register and log in to an account
- Add food entries and track calorie consumption
- Add or review exercise activities and calories burned
- Set a daily calorie goal
- Receive a notification when the goal is reached
- Choose a location using Google Maps
- Store user data locally with Room database

## Features

- User authentication flow with login and registration screens
- Daily calorie goal tracking
- Food database with built-in suggestions and custom user entries
- Exercise suggestions and user-added workout logs
- Progress visualization with a calorie progress bar
- Notification support when goal is reached
- Google Maps integration for selecting a location
- Local persistence using Room and SharedPreferences

## Tech Stack

- Kotlin
- Android Jetpack
- Room Database
- Material3 / Android Views
- Google Maps SDK
- Gradle with Kotlin DSL

## Project Structure

```text
MobileDevProject/
├── app/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/com/example/mobiledevproject/
│   │   │   │   ├── data/
│   │   │   │   ├── model/
│   │   │   │   ├── ui/theme/
│   │   │   │   ├── MainActivity.kt
│   │   │   │   ├── LoginActivity.kt
│   │   │   │   ├── RegisterActivity.kt
│   │   │   │   ├── FoodEntryActivity.kt
│   │   │   │   ├── MapActivity.kt
│   │   │   │   └── LauncherActivity.kt
│   │   │   ├── res/
│   │   │   └── AndroidManifest.xml
│   │   ├── test/
│   │   └── androidTest/
│   └── build.gradle.kts
├── build.gradle.kts
├── gradlew
├── gradlew.bat
├── settings.gradle.kts
├── gradle.properties
├── gradle/
└── README.md
```

## Core Screens

- Login screen
- Registration screen
- Main dashboard
- Food entry form
- Exercise tracking panel
- Map-based location picker

## Getting Started

### Prerequisites

- Android Studio
- JDK 11 or newer
- Android SDK with API level 35 configured
- A Google Maps API key for map functionality

### Clone the repository

```bash
git clone https://github.com/ilianadeleke/MobileDevProject.git
cd MobileDevProject
```

### Open in Android Studio

1. Open Android Studio
2. Select Open an existing project
3. Choose the cloned `MobileDevProject` folder
4. Let Gradle sync the project

### Run the app

```bash
./gradlew assembleDebug
./gradlew installDebug
```

Or run directly from Android Studio using an emulator or a physical Android device.

## Notes

- The app uses the Google Maps SDK and requires valid Google Play Services / Maps configuration.
- Data is stored locally on the device for demo and personal tracking purposes.
- User preferences are stored using `SharedPreferences`, while food and exercise entries are saved via Room.

## License

This project is currently unlicensed. If you plan to distribute or reuse it, consider adding an open-source license.

## Author

Created by `ilianadeleke`.
