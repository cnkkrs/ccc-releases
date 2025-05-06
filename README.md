# CCC Installation Guide

## Installation Instructions

1. Open the `CCC-1.0.0-arm64.dmg` file.
2. Drag and drop `CCC.app` into your **Applications** folder.

## Bypassing macOS Quarantine

As this app does not yet have an Apple Developer ID, macOS may block it from running due to its quarantine restrictions. Follow these steps to resolve this:

### Option A: Use the Provided Script
1. Run the `enableCCCapp.command` file included with the app.
2. This script should remove the quarantine, allowing you to launch `CCC.app`.

### Option B: Manual Quarantine Removal
If Option A does not work, you can manually remove the quarantine by running the following command in **Terminal**:

```bash
xattr -dr com.apple.quarantine /Applications/CCC.app
```

**Note**: If you installed `CCC.app` in a different location, replace `/Applications/CCC.app` with the correct path to the app.

## First-Time Setup
Upon launching `CCC.app` for the first time, macOS will prompt you to grant **Accessibility Permissions**. Follow these steps:
1. Grant the requested permissions.
2. The app should restart automatically. If it does not, restart it manually.

## Configuring Zoom Settings
To ensure `CCC.app` works correctly with the standalone Zoom app, configure the Zoom keyboard shortcut settings to be as shown in [this video](https://drive.google.com/file/d/1QZlFtiKjm0XJG_CuDoZTkLM_VPcWqM8i/view). Or you can follow these steps:

1. Open the Zoom app and navigate to **Settings** > **Keyboard Shortcuts**.
2. Configure the following shortcuts:
   - **Mute/unmute my audio**:
     - Set the shortcut to **Shift + Cmd + A**.
     - Check the **Enable global shortcut** checkbox.
   - **Start/stop video**:
     - Set the shortcut to **Shift + Cmd + V**.
     - Check the **Enable global shortcut** checkbox.
3. Save your changes.

## Using the App
- You can quit the app using the **system tray icon**.
- The app currently supports only the **standalone Zoom app** (not browser-based Zoom) and is compatible with **macOS** only.

## Feedback
I'd love to hear your thoughts! Please share feedback about:
- Your device
- The app’s performance
- Any suggestions for improvement
