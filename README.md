# Phantom Peak Countdown — app icon update

Upload these files/folders to the root of the existing GitHub Pages repository:

- `index.html` — updated with favicon / PWA metadata
- `manifest.webmanifest` — web-app manifest
- `icons/` — favicon and home-screen icon set

Keep the existing `Assets/` folder already in the repo.

Included icon sizes:
- 16×16 favicon
- 32×32 favicon
- 180×180 Apple touch icon
- 192×192 Android/PWA icon
- 512×512 Android/PWA icon
- 512×512 maskable icon

When someone uses "Add to Home screen", the app name will display as **Phantom Peak Countdown**.


## iPhone portrait access-bar fix

On portrait phones up to 600px CSS width, each access card now uses three rows:
1. release time
2. access group
3. countdown / ACCESS OPEN

This prevents the group name and countdown from overlapping the release time on iPhone/Safari.

The override is scoped only to narrow portrait screens. Desktop, laptop, landscape, and larger-tablet layouts are unchanged.
