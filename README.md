# HearingVault Web Repository

This repository contains the files needed to create a simple landing page and host your `app-ads.txt` file for AdMob verification using **GitHub Pages**.

## Files Included

1. **`index.html`**: A professionally designed landing page for the HearingVault app.
2. **`privacy-policy.html`**: The privacy policy required for Google Play Store compliance.
3. **`app-ads.txt`**: The configuration file required by Google AdMob to verify your app's ownership and prevent ad fraud.

## How to Host This on GitHub Pages

1. **Create a Repository:**
   - In GitHub, create a new public repository and name it (e.g., `hearingvault-web` or `yourusername.github.io`).

2. **Upload These Files:**
   - Drag all the files in this folder (`index.html`, `privacy-policy.html`, `app-ads.txt`, `README.md`) into your new GitHub repository and click **Commit changes**.

3. **Enable GitHub Pages:**
   - In the repository on GitHub, go to **Settings** -> **Pages**.
   - Under **Source**, select **Deploy from a branch**.
   - Under **Branch**, select `main` (or `master`) and leave the folder as `/ (root)`.
   - Click **Save**.

4. **Update App Credentials:**
   - Edit the `app-ads.txt` file to replace `pub-XXXXXXXXXXXXXXXX` with your actual AdMob Publisher ID.
   - Go to Google Play Console and update your website and privacy policy URLs with your new GitHub pages link (`https://yourusername.github.io/hearingvault-web/`).
   - AdMob will scan the `app-ads.txt` URL to verify your AdMob integration automatically.
