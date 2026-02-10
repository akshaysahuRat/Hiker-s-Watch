## Project Overview

Hiker's Watch is an Android Studio project built using the Gradle build system. The app is structured to handle location-based data, providing hikers with critical information during their treks.

## Tech Stack

Platform: Android 


Build System: Gradle (v7.4.1) 


Language Compatibility: Java/Kotlin (via Android Gradle Plugin) 

Modern Tooling: Uses AndroidX libraries and non-transitive R classes for optimized builds and smaller APK sizes.

## Project Structure
Below are the key configuration files included in this repository:


app/: The main application module containing your source code and resources.


build.gradle (Project-level): Defines the global build configurations and plugin versions (Android Application and Library plugins).


settings.gradle: Manages project-wide settings, including repository management (Google, Maven Central) and module inclusion.

gradle.properties: Contains JVM arguments (configured for 2048m heap size) and Android-specific flags like android.useAndroidX=true.


gradlew / gradlew.bat: Executable scripts for running Gradle commands on Unix-based systems and Windows, ensuring build consistency across environments.

## Getting Started
#### Prerequisites
Android Studio: Ensure you have the latest version of Android Studio installed.


Java Development Kit (JDK): Make sure your JAVA_HOME environment variable is correctly set to your Java installation path.

Android SDK: The project is configured to look for the SDK in your local environment.

#### Installation
Clone the repository to your local machine:

Bash
git clone https://github.com/your-username/hikers-watch.git
Open the project in Android Studio.

The IDE will automatically sync the Gradle files. If it doesn't, go to File > Sync Project with Gradle Files.

## Build & Run
To build the project from the command line:

For Windows:

Bash
gradlew.bat assembleDebug
For Unix/macOS:

Bash
./gradlew assembleDebug
## Important Notes

Local Configuration: The local.properties file is used for local SDK paths and should not be checked into version control. It is currently ignored by the .gitignore file to protect local machine settings.


Dependencies: All dependencies are resolved through Google’s Maven repository and Maven Central.

## License
This project includes Gradle wrapper scripts licensed under the Apache License, Version 2.0.
