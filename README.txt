# HabitQuest PWA

## What is included
- Installable Android/browser PWA
- Offline app shell through a service worker
- Good/bad habit logic
- 5/10/15 HP difficulty
- One answer per habit per day
- Local persistence
- Daily progress percentage
- Calendar
- Daily/weekly/monthly analytics
- Notification permission
- Service-worker notification support

## IMPORTANT: hosting
A PWA/service worker must normally be served from HTTPS (localhost is also allowed for testing).

You can upload these files to a static HTTPS host such as GitHub Pages, Netlify, Vercel, Cloudflare Pages, or your own HTTPS website.

Open the HTTPS address on Android Chrome, then use:
Chrome menu -> Add to Home screen / Install app.

## Notifications
The app requests notification permission and can show notifications through the service worker.

A browser page can check for the 21:00 reminder while the app is running. However, a normal PWA cannot guarantee an exact scheduled notification while the browser/app is completely closed on every Android/browser combination.

For guaranteed background push notifications at a chosen time, add a push backend (for example Web Push with VAPID or Firebase Cloud Messaging). The current project is structured so that can be added later without rebuilding the habit system.
