# Smart Alarm

A premium, offline-capable **Smart Alarm** web app (PWA). Built and tested end to end.

## Features
- Create, edit, delete alarms; multiple alarms; on/off toggle; labels
- Repeat days (weekly) and one-time alarms
- Live clock, next-alarm countdown, 12/24-hour format
- Ringing screen with **Stop** and **Snooze 5 min**
- Alarm history, duplicate prevention, invalid-input handling
- Data saved in localStorage (survives refresh); works offline (PWA)
- Mobile-first, dark UI, accessible (ARIA, keyboard, reduced-motion)

## Files
- `index.html` - the app (served over http/https, with the files below)
- `manifest.webmanifest`, `sw.js`, `icon-192.png`, `icon-512.png` - PWA files
- `standalone.html` - **single-file** version (open directly in any browser)

## Run it
- **Quick:** open `standalone.html` in Chrome.
- **As a real installable app:** host this folder over HTTPS (drag it onto netlify.com/drop), open the link on your phone, then tap "Install app".

## Tested
15/15 checks passed in a real (headless Chromium) browser: create, edit, delete, toggle,
multiple, repeat, invalid input, duplicate, refresh persistence, 12/24 toggle,
mobile + desktop, ring, snooze, stop, and no console errors.

## Known limitations
- Sound (beep) was not verified in the headless test - check it on a real device.
- Midnight / 7-day rollover and real-device install are not yet tested.
