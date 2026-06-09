# MediaVault

A modern, high-performance media player for Android built with Jetpack Compose and Material 3.

## Features

- **Audio Player** — Full-featured music player with playback controls, seek, shuffle, repeat, and speed control
- **Video Player** — Gesture-driven video player with brightness, volume, and seek controls
- **Equalizer** — 10-band manual equalizer with preset support
- **Playlists** — Create, edit, and manage custom playlists
- **Favorites** — Mark songs as favorites for quick access
- **Tab Navigation** — Swipeable tabs: Songs, Albums, Playlists, Favorites
- **Dark Theme** — Built-in AMOLED black theme for dark environments
- **Album Art** — Async image loading with Coil, animated rotation on playback
- **Mini Player** — Persistent mini player overlay when playing from any screen
- **Media3/ExoPlayer** — Powered by AndroidX Media3 for reliable playback

## Tech Stack

| Layer | Technology |
|---|---|
| UI | Jetpack Compose + Material 3 |
| Architecture | MVVM + Clean Architecture |
| DI | Hilt |
| Database | Room (SQLite) |
| Media | ExoPlayer (Media3) |
| Images | Coil |
| Navigation | Navigation Compose |
| Persistence | DataStore Preferences |
| Async | Kotlin Coroutines + Flow |
| Build | Gradle KTS + Version Catalog |

## Minimum Requirements

- **Android 8.0** (API 26) or higher
- **Target SDK**: 35

## Building

```bash
# Clone the repository
git clone https://github.com/Playboy-gg/MediaVault.git
cd MediaVault

# Build debug APK
./gradlew assembleDebug

# Build release APK
./gradlew assembleRelease
```

## In-App Update Checker

MediaVault checks for updates automatically on launch by querying the GitHub Releases API. If a newer version is found, a Material 3 dialog is shown with release notes and a direct download link.

The expected API response format is documented in [`github_release_sample.json`](github_release_sample.json).

## License

© 2026 Playboy-gg. All rights reserved.
