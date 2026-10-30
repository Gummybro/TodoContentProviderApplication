# To-do Content Provider

Java Android coursework project exploring SQLite storage and a content provider for tasks.

## What is included

- Defines a task contract and content URI.
- Creates a SQLite task table with sample records.
- Includes a query implementation and task-row layout.

## Current status

The adapter source is unfinished and does not compile. The activity does not load tasks into the RecyclerView, and provider insert/update/delete methods are placeholders. Complete the adapter, add an explicit RecyclerView dependency, and wire the task list before running.

## Development setup

- Android Studio with a Gradle JDK compatible with Android Gradle Plugin 8.8 (JDK 17).
- Android SDK Platform 35.
- A device or emulator running Android API 24 or newer.
- Internet access for the initial Gradle dependency download.

1. Clone this repository.
2. Open the repository root in Android Studio.
3. Let Gradle sync and install any requested SDK components.
4. Resolve the limitations above where applicable, then select the `app` run configuration.

## Build and check

From the repository root, after fixing any source blockers:

```powershell
.\gradlew.bat assembleDebug
.\gradlew.bat testDebugUnitTest
.\gradlew.bat lintDebug
```

On macOS or Linux, use `bash ./gradlew` in place of `.\gradlew.bat`.

These commands are provided for local verification; a successful build or device run has not been verified as part of the repository documentation cleanup. The included example tests are starter tests, not full behavior coverage.

## Usage

The intended app displays tasks from the local content provider. The current database includes sample tasks for development.

## Project layout

| Path | Purpose |
| --- | --- |
| `app/src/main/java/` | Java source |
| `app/src/main/res/` | Layouts, strings, and drawable resources |
| `app/src/main/AndroidManifest.xml` | Application components and permissions |
| `app/build.gradle.kts` | Android module configuration |
| `gradle/libs.versions.toml` | Dependency and plugin versions |
