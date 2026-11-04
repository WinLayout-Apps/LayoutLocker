# Layout Locker

**Remembers where you want your windows and keeps them there.**

Layout Locker (formerly WinLayout) is a small Windows app that sits in your system tray and puts every window back where you left it: after a restart, when a monitor is plugged in or removed, or when an app opens a panel you had moved.

**[Download the latest version](../../releases/latest)** (Windows 10 or 11, 64-bit. No .NET install needed.)

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/WinLayout)

## What it does

- Remembers the size, position and state of each app's windows and restores them automatically.
- Works across several monitors, including windows that stretch across screens.
- Handles undocked panels and tool windows, for example an image browser in a photo editor.
- Optional **Lock**: a window snaps straight back if it gets moved.
- Capture one window, or all open windows at once, and apply your rules whenever you like.
- Match windows by application and by part of the title (plain text or a regular expression), and reorder rules to set priority.
- Light, dark, or the same as Windows (your choice in App Settings), optional keyboard shortcuts, and an option to start with Windows.
- Tells you when a newer version is out (you can switch this off). It never installs anything by itself.

## User guide

The full guide is a PDF: **[Layout Locker user guide](LayoutLocker-User-Guide.pdf)**. It covers installing, capturing windows, rules, locking, several monitors, every setting and troubleshooting.

## Getting started

1. Download and run the installer from the latest release. By default it installs just for you, so it doesn't need administrator rights. If you have WinLayout installed, run it over the top: that updates it and keeps your rules.
2. Open Layout Locker from the Start menu, or find its icon in the system tray.
3. Put a window where you want it, then click **Capture Single Window** (or **Capture All Open Windows**).
4. The next time that window opens, Layout Locker puts it back. Use a rule's cog to fine-tune it, and tick **Lock** to keep a window in place.

## Privacy

Everything runs on your PC, and Layout Locker doesn't collect any data about you. Its only network use is a quick check on GitHub for a newer version, when it starts and then every few hours. That request carries nothing about you or your PC, and you can switch it off in App Settings. Links in the About box, such as Ko-fi, and its **Report a problem** and **Request a feature** buttons (which open a short web form, with your Layout Locker version in the address) open in your browser only when you click them, and nothing is sent unless you submit a form. Your rules and settings are stored in `%AppData%\Layout Locker`.

## Windows and antivirus warnings

Layout Locker isn't code-signed yet, so:

- Windows may show **"Windows protected your PC / unknown publisher"**. Click **More info**, then **Run anyway**.
- A virus scanner may occasionally flag a new, unsigned program with a generic detection. These are false positives, and I report them when they happen.

Each release lists the **SHA-256** of its installer. To check a download, run this in PowerShell and compare the result:

```powershell
Get-FileHash .\LayoutLocker-Setup-<version>.exe -Algorithm SHA256
```

## Uninstall

Use **Settings, Apps** in Windows, or **App Settings, Uninstall Layout Locker** inside the app. You'll be asked whether to keep your saved rules.

## Questions and problems

Found a bug, or have a question or an idea? In Layout Locker, open **About** and click **Report a problem** or **Request a feature**. Each opens a short form in your web browser, with your Layout Locker version already filled in. Please say what you were doing. If you're having problems downloading or installing the app please use this [contact form](https://tally.so/r/VpG2Vl?software_name_version=Layout%20Locker).

## Support

Layout Locker is made in my spare time. If it's useful to you, you can support it on [Ko-fi](https://ko-fi.com/WinLayout). The money goes towards a code-signing certificate, so Windows stops showing the unknown-publisher warning.

## Licence

Copyright (c) 2026 Martin Lewis. Layout Locker is free to use. It is provided as is, without warranty of any kind.
