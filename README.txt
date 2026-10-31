BuzzReady  ·  Installable web app
====================================

What this folder is
-------------------
The complete app, ready to put on the web so quizzers can install it on
their phones and tablets like an app (own icon, full screen, works offline).

  index.html             the app
  manifest.webmanifest   app name, colours and icons for the home screen
  sw.js                  offline support
  icons/                 app icons (all sizes)
  fonts/, fonts.css      the app's fonts, included so it works fully offline

Step 1 · Put it online (pick one, both are free)
------------------------------------------------
A) Netlify Drop (easiest, about 2 minutes)
   1. Go to https://app.netlify.com/drop
   2. Drag this whole folder onto the page.
   3. You get a web address like https://buzzready.netlify.app
      (sign up free to keep it and to choose the name).

B) GitHub Pages
   1. Create a free GitHub account and a new public repository, e.g. "buzzready".
   2. Upload all files in this folder (keep the icons folder).
   3. Settings → Pages → Source: "Deploy from a branch", Branch: main, folder: / (root).
   4. After a minute the app is at https://YOUR-NAME.github.io/buzzready/

The address must start with https:// for install and offline to work.

Step 2 · Install it on a device
-------------------------------
iPhone / iPad (Safari):  open the address → Share button → "Add to Home Screen" → Add.
Android (Chrome):        open the address → menu (⋮) → "Install app" (or "Add to Home screen").
Computer (Chrome/Edge):  open the address → install icon at the right of the address bar.

Open it once while online; after that it also works with no internet.

Updating the app later
----------------------
1. Replace index.html with the new version.
2. In sw.js change  VERSION = 'buzzready-v1'  to  'buzzready-v2'  (v3, v4 … each time).
3. Upload again. Devices pick up the new version the next time the app is opened online
   (sometimes it takes a second open).

Good to know
------------
- Stars, filters and saved Quote Builder results stay on each device.
- Speech input (Buzz In) and read-aloud (Listen & Buzz) use the device's own speech features.
- The questions come from the JBQ Fact Pak. Keep the address private to your team unless you
  have the publisher's permission to share the content publicly.
