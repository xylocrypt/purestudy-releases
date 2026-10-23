# PureStudy browser extension

The PureStudy 2.3 extension for **Chrome and Edge** opens the full app in a normal browser tab. It keeps the timer running if you close the tab, then shows a notification and a badge when the block ends.

## Download

- **[PureStudy-Extension-v2.3.0.zip](https://github.com/xylocrypt/purestudy-releases/releases/download/extension-v2.3.0/PureStudy-Extension-v2.3.0.zip)**
- [SHA-256 checksum](https://github.com/xylocrypt/purestudy-releases/releases/download/extension-v2.3.0/SHA256SUMS.txt)
- [Release page](https://github.com/xylocrypt/purestudy-releases/releases/tag/extension-v2.3.0)

`27125b95f8de10a17857b17842e4488903abc1b9995dd14981e9916f1f6c4794`

## Install

1. Download the ZIP and extract it. Keep the extracted folder somewhere permanent; unpacked extensions use the folder path for their identity.
2. Open `chrome://extensions` or `edge://extensions`.
3. Turn on **Developer mode**.
4. Click **Load unpacked** and select the extracted folder (the one containing `manifest.json`).
5. Pin **PureStudy** from the extensions menu. Chrome and Edge hide new extensions by default; a browser extension cannot pin itself.
6. Click the toolbar icon or press **Alt+Shift+P** to open PureStudy.

The first-run page opens automatically after installation. If the toolbar icon is pinned, it opens the app directly; otherwise it shows the exact pinning steps. Updating an unpinned install also reopens the guide.

## About the toolbar icon

The PureStudy icon lives in the **browser toolbar**, beside the address bar. It does not create a separate Windows taskbar button. A standalone taskbar app would need a PWA or desktop package, which is separate from this extension.

## Data and privacy

- Study data is stored locally in the extension under `focusstudy.v1`.
- The extension has no host permissions, content scripts, analytics, or network requests.
- `storage` keeps the app data, the tracked tab ID, and the active timer's end time.
- `alarms` schedules one local alarm for the end of a focus block or break.
- `notifications` shows a local completion notification while the app tab is closed.
- External links open only when you click them.

The extension's data is separate from the web app and Windows app. Export a JSON backup from **Settings → Export backup** before uninstalling or moving the extension folder.
