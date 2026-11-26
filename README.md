# Rider Predictor AI — Android APK build project

This is the first Android-packaging project for Rider Predictor AI.

## Build an APK using only an Android phone (GitHub Actions)

1. Download and extract `Rider_Predictor_AI_Android_Build.zip` on your phone.
2. Sign in to GitHub or create an account at https://github.com.
3. Create a **public** repository named `rider-predictor-ai` (public is the simplest way to use GitHub Actions on a free account; check current GitHub plan limits).
4. In the repository, use **Add file → Upload files** and upload the project contents: `package.json`, `capacitor.config.json`, the `www` folder, and the `.github/workflows/android.yml` workflow file. Keep the folder structure exactly as shown.
5. Commit the uploaded files to the `main` branch.
6. Open the repository's **Actions** tab. Select **Build Rider Predictor AI APK** and tap **Run workflow** if it has not started automatically.
7. Wait for the workflow to finish successfully. Open the completed run, scroll to **Artifacts**, and download `rider-predictor-ai-debug-apk`.
8. Extract the artifact ZIP and tap `app-debug.apk` to install. Android may ask you to allow installs from your browser or Files app; only enable this for the trusted source you used, then turn it off afterward.

## Important
- This is a **debug APK for testing**, not a Play Store release or a signed production release.
- The app currently calculates market-implied probabilities from odds entered by the user, builds double-chance jackpot lists, and stores prediction history on the device.
- Live worldwide fixtures, team form, injuries, lineups, odds feeds, result feeds, user accounts, push notifications, and a trained AI model are **not connected yet**. They require further development and suitable data-provider access.
- The prototype must not be treated as a source of guaranteed betting outcomes.
