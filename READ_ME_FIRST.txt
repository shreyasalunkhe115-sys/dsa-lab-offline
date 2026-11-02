DSA LAB - INSTALLABLE OFFLINE APP

WHAT THIS PACKAGE DOES
This is a Progressive Web App (PWA) version of your DSA Lab HTML file.
Once a computer has opened the hosted app and installed it while online,
the app files are cached and the app can be opened offline on that computer.

IMPORTANT
- Each computer needs an initial online visit and installation.
- A PWA cannot be installed on a never-connected computer remotely.
- Keep the hosted website available for first-time installations and updates.
- The app shows your HTML content offline. Running Java programs still
  requires a Java JDK on that computer.

HOW TO PUBLISH (EASIEST: GITHUB PAGES)
1. Sign in to https://github.com or create a free account.
2. Create a new repository, for example: dsa-lab-offline
3. Set it to Public, then create the repository.
4. Open the repository and choose Add file > Upload files.
5. Upload ALL items from this folder:
   index.html
   manifest.webmanifest
   service-worker.js
   icons folder (with both PNG files)
6. Commit the uploaded files.
7. Open repository Settings > Pages.
8. Under Build and deployment, choose Deploy from a branch.
9. Select branch "main" and folder "/ (root)", then Save.
10. Wait for GitHub Pages to publish. It will show a website URL.
11. Open that URL in Google Chrome on each computer while online.
12. In Chrome, click the install icon near the right side of the address bar,
    or open Chrome menu (three dots) > Cast, save and share > Install page as app
    (wording may vary by Chrome version).
13. Click Install.
14. To test offline, turn off Wi-Fi and open DSA Lab from the desktop or
    Start menu. The first visit must finish loading while online before
    switching offline.

ALTERNATIVE HOSTING
You can also deploy this folder to a static HTTPS host such as Netlify.
Upload the folder as a site using its deploy workflow, then open the HTTPS
site URL in Chrome and install it on each computer.

TROUBLESHOOTING
- If the install option does not appear, check that the site uses HTTPS,
  the manifest and icons uploaded correctly, and service-worker.js is at
  the same site folder level as index.html.
- After changing files, reload the hosted site while online. If an old
  version remains, close the app and reopen Chrome after a refresh.
- Do not open index.html by double-clicking for PWA installation.
  Service workers require HTTPS (or localhost); use the hosted HTTPS URL.
