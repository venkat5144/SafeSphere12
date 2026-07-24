# SafeSphere — Firebase Hosting Package

This package contains a self-contained, interactive SafeSphere prototype ready for Firebase Hosting.
It does not require a Next.js build or npm dependencies for the website itself.

## Fastest deployment on Windows

1. Extract this ZIP.
2. Double-click `deploy-firebase.bat`.
3. Sign in to the Google account that owns your Firebase project.
4. Enter your Firebase **Project ID** when prompted.
5. The terminal will print the live URL after deployment.

The live URL is normally:

```text
https://YOUR_PROJECT_ID.web.app
```

## Manual deployment

Install Firebase CLI and sign in:

```bash
npm install -g firebase-tools
firebase login
```

Deploy from this folder:

```bash
firebase deploy --only hosting --project YOUR_FIREBASE_PROJECT_ID
```

## Firebase project setup

If you do not yet have a Firebase project:

1. Open Firebase Console.
2. Select **Create a project**.
3. Choose a project name such as `safesphere-community`.
4. Open **Project settings** and copy the Project ID.
5. Run the deployment command above.

## Files

- `public/index.html` — complete interactive SafeSphere website
- `public/404.html` — fallback page
- `firebase.json` — Hosting configuration and security headers
- `deploy-firebase.bat` — Windows one-click deployment
- `deploy-firebase.ps1` — PowerShell deployment
- `deploy-firebase.sh` — macOS/Linux deployment
