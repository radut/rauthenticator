# rAuthenticator

Two-factor codes on your Mac, iPhone and iPad (and Linux), with Google Authenticator import.

**Website: https://radut.github.io/rauthenticator/**

This repository holds only the **releases** and the **website**. The source code is not here.

## Downloads

The latest release always has the same file names, so these links stay valid:

| Platform | Download |
|----------|----------|
| macOS 14+ | [rAuthenticator.dmg](https://github.com/radut/rauthenticator/releases/latest/download/rAuthenticator.dmg) |
| Linux (Debian/Ubuntu, x86-64) | [rAuthenticator-amd64.deb](https://github.com/radut/rauthenticator/releases/latest/download/rAuthenticator-amd64.deb) |
| Linux (any distribution, x86-64) | [rAuthenticator-x86_64.AppImage](https://github.com/radut/rauthenticator/releases/latest/download/rAuthenticator-x86_64.AppImage) |
| iPhone & iPad | TestFlight beta, by invitation |

Each release also carries `SHA256SUMS`. Check a download with:

```bash
sha256sum --ignore-missing -c SHA256SUMS
```

Linux files appear from the first release that includes them; older releases have the DMG only.

## Website

`site/` is published to GitHub Pages by `.github/workflows/pages.yml` on every push to `main`.
