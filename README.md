<p align="center">
  <img src="https://radut.github.io/rauthenticator/screenshots/icon_256x256@2x.png" width="112" alt="">
</p>
<h1 align="center">rAuthenticator</h1>
<p align="center">
  <b>Your two-factor codes, one keystroke away.</b><br>
  A native Mac, iPhone and Linux companion to Google Authenticator. Copy your accounts from the phone to the computer
  <b>without removing them from the phone</b>, then type a few letters, press Return and paste.
</p>
<p align="center">
  <a href="https://github.com/radut/rauthenticator/releases/latest/download/rAuthenticator.dmg"><b>Download for Mac</b></a> ·
  <a href="https://radut.github.io/rauthenticator/#iphone"><b>iPhone &amp; iPad</b></a> ·
  <a href="https://github.com/radut/rauthenticator/releases/latest/download/rauthenticator_amd64.deb"><b>Linux .deb</b></a> ·
  <a href="https://github.com/radut/rauthenticator/releases/latest/download/rAuthenticator-x86_64.AppImage"><b>AppImage</b></a> ·
  <a href="https://radut.github.io/rauthenticator/">Website</a> ·
  <a href="#keyboard">Keyboard</a> ·
  <a href="#install">Install</a> ·
  <a href="#faq">FAQ</a> ·
  macOS 14, iOS and iPadOS 17, Ubuntu 24.04 (or any distro with GTK 4.14 and libadwaita 1.5) or newer
</p>

<p align="center">
  <img src="https://radut.github.io/rauthenticator/screenshots/ios-search.gif" width="300" alt="Typing acm narrows the list to Acme Cloud; a tap copies its code">
</p>

## Three apps, one authenticator

The same codes, QR formats and app lock everywhere, from one Swift codebase (`AuthenticatorCore` holds the logic all
three share). Each device keeps its own list; moving accounts between them is one scan (**Export All** on one, the
scanner on the other).

| | **rAuthenticator for Mac** | **rAuthenticator for iPhone & iPad** | **rAuthenticator for Linux** |
|---|---|---|---|
| Copy a code | type a few letters, <kbd>Return</kbd> | tap the account | type a few letters, <kbd>Return</kbd> |
| Get accounts in | viewfinder, whole screen, screen region, camera, image, paste, drop, setup key | camera, photo, setup key | whole screen, screen region, image, paste, drop, setup key |
| Google Authenticator transfers | yes, multi-code included | yes, multi-code included | yes, multi-code included |
| Lock | Touch ID or password: launch, sleep, idle, <kbd>⌘</kbd><kbd>L</kbd> | Face ID / Touch ID / passcode; the app switcher shows no codes | login password or fingerprint (polkit), or an app passphrase (AppImage): launch, session lock, sleep, idle (GNOME), <kbd>Ctrl</kbd><kbd>L</kbd> |
| Export | one account as QR, everything as transfer codes | one account as QR, everything as transfer codes | one account as QR, everything as transfer codes |
| Get it | [DMG download](https://github.com/radut/rauthenticator/releases/latest/download/rAuthenticator.dmg), macOS 14+ | Coming soon, iOS / iPadOS 17+ | [.deb](https://github.com/radut/rauthenticator/releases/latest/download/rauthenticator_amd64.deb) (Ubuntu 24.04 or newer) or [AppImage](https://github.com/radut/rauthenticator/releases/latest/download/rAuthenticator-x86_64.AppImage), x86_64 |

<a id="keyboard"></a>
## Keyboard

On the Mac there is no search box to click: switch to the app and type. The list narrows to the accounts whose
issuer or name contain every word you typed; once one is left, **Return** copies its code and clears the search, so
the next thing you type starts over. **Esc** clears it by hand. Then switch back and paste.
On Linux every shortcut is the same with <kbd>Ctrl</kbd> instead of <kbd>⌘</kbd> (Settings: <kbd>Ctrl</kbd><kbd>,</kbd>);
the viewfinder and the camera are not there yet.

| Action | Keys | | Action | Keys |
|---|---|---|---|---|
| Search | just type | | Scan with viewfinder | <kbd>⇧</kbd><kbd>⌘</kbd><kbd>F</kbd> |
| Copy the only match | <kbd>Return</kbd> | | Scan the whole screen | <kbd>⇧</kbd><kbd>⌘</kbd><kbd>S</kbd> |
| Clear the search | <kbd>Esc</kbd> | | Select a screen region | <kbd>⇧</kbd><kbd>⌘</kbd><kbd>R</kbd> |
| Hide / show codes | <kbd>⇧</kbd><kbd>⌘</kbd><kbd>H</kbd> | | Scan with camera | <kbd>⇧</kbd><kbd>⌘</kbd><kbd>K</kbd> |
| Lock now | <kbd>⌘</kbd><kbd>L</kbd> | | Import QR image | <kbd>⌘</kbd><kbd>O</kbd> |
| Settings | <kbd>⌘</kbd><kbd>,</kbd> | | Paste QR image | <kbd>⇧</kbd><kbd>⌘</kbd><kbd>V</kbd> |
| Export all to Google Authenticator | <kbd>⇧</kbd><kbd>⌘</kbd><kbd>E</kbd> | | Enter setup key | <kbd>⌘</kbd><kbd>N</kbd> |

## A look around

<p align="center">
  <img src="https://radut.github.io/rauthenticator/screenshots/ios-list.png" width="200" alt="The list of accounts with their codes and countdown rings">
  <img src="https://radut.github.io/rauthenticator/screenshots/ios-export.png" width="200" alt="One account as a QR code and setup key">
  <img src="https://radut.github.io/rauthenticator/screenshots/ios-exportAll.png" width="200" alt="All accounts as Google Authenticator transfer codes">
</p>
<p align="center">
  <img src="https://radut.github.io/rauthenticator/screenshots/ios-manual.png" width="200" alt="Enter a setup key">
  <img src="https://radut.github.io/rauthenticator/screenshots/ios-edit.png" width="200" alt="Edit an account">
  <img src="https://radut.github.io/rauthenticator/screenshots/ios-settings.png" width="200" alt="Settings: Face ID lock and hide codes">
</p>
<p align="center">
  <img src="https://radut.github.io/rauthenticator/screenshots/ipad-list.png" width="640" alt="The same list on iPad">
</p>

The list, one account as a QR code, everything as Google Authenticator transfer codes, a typed setup key, editing,
and the settings; then the iPad. All pictures use made-up accounts, with the codes, QR codes and setup keys blurred.

## Install

| Platform | How | Requires |
|---|---|---|
| **Mac** | [Download the DMG](https://github.com/radut/rauthenticator/releases/latest/download/rAuthenticator.dmg), open it, drag **rAuthenticator** onto **Applications**. Signed with Developer ID and notarized by Apple, so it opens like any other downloaded app. | macOS 14 or newer, Apple silicon or Intel |
| **iPhone & iPad** | Coming soon. | iOS / iPadOS 17 or newer |
| **Linux** | [.deb](https://github.com/radut/rauthenticator/releases/latest/download/rauthenticator_amd64.deb): `sudo apt install ./rauthenticator_amd64.deb` (pulls in GTK 4, libadwaita, libsecret, zbar, qrencode; the app lock uses polkit). [AppImage](https://github.com/radut/rauthenticator/releases/latest/download/rAuthenticator-x86_64.AppImage): `chmod +x`, then run it (everything bundled; the app lock uses a passphrase). | Ubuntu 24.04 or newer (glibc 2.39+), x86_64 |

### From your phone to your Mac in two minutes

Your phone keeps its accounts: Google Authenticator's export only shows them.

1. In Google Authenticator on the phone: **☰ → Transfer accounts → Export accounts**, and pick all accounts or a few.
2. In rAuthenticator: **+ → Scan with Camera…** and hold the phone up (on the iPhone: **+ → Scan QR Code**), or on
   the Mac mirror the phone and use the viewfinder.
3. Keep scanning until the banner says all codes are in. From then on, switch to the app and just start typing.

## Security at a glance

Boring, on purpose: no server, no account, no sync service, no third-party code.

- **In your Keychain.** Secrets live in the login Keychain, never in plain files. The previous list is kept too, so
  one bad edit can be undone.
- **A careful clipboard.** Copied codes stay on this device (no Universal Clipboard), are flagged so clipboard
  managers skip them, and vanish after 60 seconds.
- **Export asks first.** A setup key is as sensitive as a password, so showing one or exporting everything needs Touch
  ID, Face ID or the device password.
- **Hide and lock.** Blur the codes for screen sharing; lock with Touch ID / Face ID on launch, sleep, idle or
  <kbd>⌘</kbd><kbd>L</kbd>.
- **Never online.** The apps make no network connections at all: no analytics, no update checks, no cloud backup.
- **Native and small.** SwiftUI, about 2.5 MB to download, tested against the RFC 4226/6238 vectors and Google's
  transfer format.

The details are in [Security notes](#security-notes).

## Features

- Imports Google Authenticator "Transfer accounts" QR codes (all accounts or a selection) and plain
  `otpauth://` QR codes from any service.
- Five ways to get a QR code in: **hold the viewfinder window over it**, **scan the whole screen**,
  **select a screen region**, **use a camera** (built-in, USB, or your iPhone as Continuity Camera),
  or **open / paste / drop an image**.
- Click an account → its code is on the clipboard. It is copied for this Mac only (never synced by
  Universal Clipboard), flagged so clipboard managers skip it, and cleared again after a minute.
- Just start typing to search: the list narrows to the accounts whose issuer or name contain every
  word you typed. **Return** copies the code once a single account is left, **Esc** clears the search.
- **Hide codes** with the eye button (or View → Hide Codes): the list shows blurs instead of digits,
  and clicking still copies.
- Optional **app lock** (Settings, ⌘,): Touch ID or your login password is needed when the app opens
  and after the Mac sleeps or its screen is locked. ⌘L locks it right away. Optionally it also locks
  after the Mac has been idle (no keyboard or mouse input) for 1–60 minutes; that is off by default.
- Time-based (TOTP) and counter-based (HOTP) codes, SHA-1/256/512, 6–8 digits, custom periods.
- Secrets are stored in your login Keychain, never in plain files. The previous version of the list is
  kept in a second Keychain item before every change, so one bad edit can be undone.
- Export back out (behind Touch ID or your login password): one account as an `otpauth://` QR code,
  or everything as Google Authenticator transfer QR codes.

Requires macOS 14 or newer. No third-party dependencies.

## Getting accounts from your phone

1. In Google Authenticator on the phone: menu (☰) → **Transfer accounts** → **Export accounts**,
   pick all accounts or just the ones you want, and the phone shows one or more QR codes.
2. On the Mac, in rAuthenticator, click **+** and choose one of:
   - **Scan with Camera…** and hold the phone up to the camera (easiest with the iPhone as
     Continuity Camera, or any webcam).
   - **Scan with Viewfinder…** opens a small see-through window: drag it over a QR code anywhere on
     your screen and the code inside its frame is read automatically. Only what is inside the frame
     is looked at.
   - **Scan Screen for QR Code** if the code is visible on your Mac's screen (mirrored phone, a
     screenshot, a shared screen in a video call, …).
   - **Select Screen Region…** to draw a rectangle around a code with the system crosshair.
   - **Import QR Code from Image…**, **Paste QR Code Image**, or drop an image onto the window.
3. If the export has several QR codes, keep scanning: a banner tracks "Received 1 of 3 QR codes" until
   all are in, and the camera sheet stays open between codes. Accounts that already exist (same secret)
   are skipped, so re-scanning is harmless, even after you renamed them here.

Your phone keeps its accounts; export only *shows* them. For a single new service, just scan the
service's own QR code, or click **+ → Enter Setup Key…** and type the key.

## Permissions

macOS asks the first time a feature needs it:

| Feature | Permission | Where to change it |
|---|---|---|
| Viewfinder / Scan Screen / Select Screen Region | Screen & System Audio Recording | System Settings → Privacy & Security |
| Scan with Camera | Camera | System Settings → Privacy & Security |

If a scan says permission is missing, grant it and try again (macOS sometimes needs the app to be
reopened after the first grant).

## Security notes

- Secrets live in a Keychain item (service `com.radut.authenticator-companion`, account `accounts`) as
  JSON, with the previous version in `accounts.previous`; delete both with Keychain Access to wipe the app.
- If the saved list can't be read (for example you denied the Keychain prompt), the app refuses to
  save anything until a read succeeds, so it can never overwrite your accounts with an empty list.
- Exported QR codes and setup keys are as sensitive as passwords: anyone who sees them can generate
  your codes. That is why export asks for Touch ID or your password first.
- The app lock hides the accounts behind Touch ID / your password; it is a screen lock, not extra
  encryption. The secrets stay in the login Keychain as before, protected by your macOS login.
- Copied codes are placed on the clipboard for this Mac only, flagged with
  `org.nspasteboard.ConcealedType` for clipboard managers, and cleared after 60 seconds.
- "Scan Screen" imports every otpauth QR code visible on any display; check the toast and the list
  afterwards if other people's windows were on screen.
- Google's transfer format can't carry 7-digit codes or periods other than 30 s; such accounts are
  left out of "Export All" (the sheet says which) and can be shown individually instead.

## FAQ

**Does my phone lose its accounts?** No. Google Authenticator's export only shows QR codes; the accounts stay on the
phone. You end up with the same codes on both.

**Is the Mac download safe to open?** Yes: the DMG and the app are signed with a Developer ID and notarized by Apple,
so macOS opens them without warnings. Download it only from the GitHub release.

**Why does it ask for Screen Recording or Camera?** Only the scanners need them: the viewfinder, screen and region scans
read your screen, the camera scan reads the camera. Nothing else uses them, and nothing leaves the Mac.

**Can I move accounts between the Mac and the iPhone?** Yes, the same way as from Google Authenticator: **Export All**
on one shows transfer QR codes, the scanner on the other reads them.

**Which codes work?** Time-based (TOTP) and counter-based (HOTP), SHA-1, SHA-256 and SHA-512, 6 to 8 digits, any
period. Google's transfer format can't carry 7-digit codes or periods other than 30 s; those export one by one instead.

**How do I wipe it?** Delete the app's two items in Keychain Access (search for "authenticator"), then the app.

Not affiliated with Google. Google Authenticator is a trademark of Google LLC.

## Downloads

[All releases](https://github.com/radut/rauthenticator/releases) · [Website](https://radut.github.io/rauthenticator/). This repository holds only the releases and the website.
