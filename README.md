# Velvet Home

An ad-free, Apple TV-style home screen for Android TV. **393 KB.** No ads, no telemetry, no bloat.

Built on [CleanYourTV](https://github.com/Gathin23/cleanyourtv) (MIT) and extended with a glass UI, a wallpaper engine and an in-app image browser.

---

## Screenshots

**One pencil, every setting.** Wallpaper, layout editing, hidden apps, restoring them, and the launcher's own settings all sit behind a single pencil in the top bar.

![Pencil menu open under the top bar](screenshots/menu-pencil.png)

| Layout editing | App library |
|---|---|
| ![Moving and hiding tiles in layout edit mode](screenshots/edit-layout.png) | ![App library with add-to-home toggles, 39 apps](screenshots/app-library.png) |

**Home.** A large clock, a dock, and a glass highlight that springs to whatever you focus. Hide the dock and it becomes a plain, quiet grid.

| Home with the dock | App grid and the library tile |
|---|---|
| ![Home screen with the dock](screenshots/home-dynamic.png) | ![App grid with the App library tile](screenshots/home-black.png) |

**Wallpaper.** Browse folders, see thumbnails at their real shape, then set or delete a picture without leaving the launcher.

| Wallpaper browser | Image preview |
|---|---|
| ![Folder browser showing image thumbnails at their real aspect ratios](screenshots/wallpaper-browser.png) | ![Full-size preview with Set as current wallpaper and Delete image](screenshots/wallpaper-preview.png) |

**Settings.** A translucent page that floats over Home, with a glass slider for the column count.

![Launcher settings](screenshots/settings.png)

## Features

- **Apple TV-style home** — big clock, date, dock with a springing glass highlight
- **Screensaver-free** — no ads, no recommendations, no sponsored rows
- **App library** — every installed app, TV or phone, with add-to-home / hide toggles
- **Layout editing** — move tiles with the D-pad; hide without uninstalling
- **Wallpaper engine** — use an image, or rotate a whole folder on an interval
- **In-app browser** — folders and image thumbnails at their true aspect ratio, no file-manager required
- **Image preview** — set as wallpaper or delete, without leaving the launcher
- **Glass UI throughout** — menus, dialogs and settings share one material

## Install

```bash
adb install -r velvet-home-v1.0.apk
adb shell cmd package set-home-activity com.gathin.tvhome/.MainActivity
```

Requires **Android 8.0+** (minSdk 26). Tested on a TCL Android TV (API 28).

## Size

| | |
|---|---|
| APK | **393,466 bytes (384 KB)** |
| Launcher original | 374,957 bytes (366 KB) |
| Overhead for everything above | **+5.0%** |

## Credits

Forked from [CleanYourTV](https://github.com/Gathin23/cleanyourtv) by Gathin23, MIT licensed. The launcher, glass material and motion system build on that work.
