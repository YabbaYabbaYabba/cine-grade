Cine Grade - installable web app
================================

Files (keep them together, same folder structure):
  index.html            the app
  manifest.webmanifest  app name, icon and full-screen settings
  sw.js                 offline cache
  icons/                app icons

1. Host it
   Upload the whole folder to any web server that serves it over HTTPS.
   HTTPS is required: without it the phone will not enable offline use.
   No server-side code, database or build step is needed.

2. Install on iPhone
   Open the address in Safari, tap Share, then "Add to Home Screen".
   Launch it once from the Home Screen icon while online. After that it works offline.

3. Save to Photos
   Tap Save JPEG or Save PNG, then choose "Save Image" in the share sheet.

Updating
   When you replace the files, change VERSION in sw.js (for example to "cine-grade-v2").
   Phones fetch the new version the next time the app is opened online.

Privacy
   Photos are processed in the browser on the device. The app makes no network
   requests other than loading its own files from your server.
