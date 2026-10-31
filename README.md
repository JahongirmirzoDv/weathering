# Map-Based Weather for Android

A Kotlin Android prototype that lets a user choose coordinates on Google Maps and request weather information for that location.

## What it demonstrates

- A draggable map marker and coordinate handoff to a weather screen.
- Google location permission and location-settings flows.
- A Retrofit weather endpoint accepting latitude, longitude, units, and app ID.
- ViewModel-backed weather presentation with XML layouts.

## Source guide

- [app/src/main/java/com/example/weatherapptest/MapsActivity.kt](app/src/main/java/com/example/weatherapptest/MapsActivity.kt) — map and location selection
- [app/src/main/java/com/example/weatherapptest/ViewActivity.kt](app/src/main/java/com/example/weatherapptest/ViewActivity.kt) — weather detail screen
- [app/src/main/java/com/example/weatherapptest/MainViewModel.kt](app/src/main/java/com/example/weatherapptest/MainViewModel.kt) — weather request state
- [app/src/main/java/com/example/weatherapptest/retrofit/ApiService.kt](app/src/main/java/com/example/weatherapptest/retrofit/ApiService.kt) — weather request contract

## Open the project

The checked-in build uses Android Gradle Plugin 7.0.4, Kotlin 1.6.10, Gradle 7.0.2, compile/target SDK 31, and minimum SDK 21.

Open the repository in Android Studio and let it use the checked-in Gradle configuration. Select the `app` configuration and an Android device or emulator meeting the minimum SDK requirement.

## Service configuration

Google Maps uses the `google_maps_key` resource under the debug/release source sets. Weather requests also require a provider app ID. Configure credentials for services you control rather than reusing checked-in values. The current manifest needs network-permission review before API calls can work; this documentation update does not change the application.

## Project status

This repository is a learning sample. Build and device behavior have not been verified as part of this documentation update.

