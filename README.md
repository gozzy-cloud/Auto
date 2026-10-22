# AutoRide Local — Android APK project

This wraps the supplied HTML demo in a Capacitor Android app. It keeps the original HTML/CSS/JavaScript UI.

## Important demo limitations
- The listed drivers and contact details are sample/demo data. Do not treat them as verified real drivers.
- Registration and status changes are stored only in the current app session; they do not sync between devices and may reset after restarting.
- The page uses Tailwind CSS, Font Awesome, and Google Fonts from CDNs, so those visual assets require an internet connection.
- This is a test/debug APK, not a Play Store release.

## Build the APK using a phone and GitHub Actions

1. In your phone browser, create a new GitHub repository (for example `autoride-local-android`).
2. Extract this ZIP using your phone's file manager.
3. Upload the **contents** of this extracted folder to the repository, preserving the `.github/workflows/build-apk.yml` path. GitHub's web upload flow may be awkward on mobile; if needed, switch the browser to Desktop site.
4. Commit the files to the `main` branch.
5. Open the repository's **Actions** tab. Select **Build AutoRide Local APK**, then tap **Run workflow** if it has not already started from the push.
6. Wait for the workflow to finish successfully.
7. Open the completed workflow run, find **Artifacts**, and download `AutoRide-Local-debug-APK`.
8. Extract the downloaded artifact ZIP and tap `app-debug.apk` to install it.
9. If Android blocks installation, allow your browser or file manager to **Install unknown apps** for this one installation, then retry. Only install APKs you built or trust.

## If GitHub Actions is unavailable
You will need a compatible cloud build service or a computer with Node.js, Java, and Android build tools. This ZIP itself is the project source; it is not the compiled APK.
