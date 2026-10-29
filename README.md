# HearingVault Web — GitHub Pages source

This folder holds the files published for Google Play and AdMob:

- **Canonical site:** `https://devd32033-gif.github.io/hearingvault/`
- Publisher: **AACrazy Enterprises** — contact `aacrazyenterprises@gmail.com`

## Files

| File | Live URL | Purpose |
|---|---|---|
| `index.html` | `/hearingvault/` | Landing page with the legal resource links |
| `privacy-policy.html` | `/hearingvault/privacy-policy.html` | Full policy: data collected, storage, AI, advertising + app-ads.txt verification, retention and deletion |
| `delete-account.html` | `/hearingvault/delete-account.html` | Play-required account & data deletion instructions |
| `app-ads.txt` | `/hearingvault/app-ads.txt` | AdMob Authorized Digital Sellers file |

The same four files are mirrored in the repository's `/docs` folder. The two copies are kept
byte-identical — check with `Get-FileHash` before pushing.

## Deploying

The site is served from the **`hearingvault`** GitHub repository. To publish a change:

1. Edit the files here, copy them into `/docs`, and commit.
2. Push to the branch Pages publishes (`main`).
3. Wait for the build (~1 minute), then hard-refresh and check:
   - `https://devd32033-gif.github.io/hearingvault/privacy-policy.html`
   - `https://devd32033-gif.github.io/hearingvault/delete-account.html`
   - `https://devd32033-gif.github.io/hearingvault/app-ads.txt`

An older duplicate site exists at `https://devd32033-gif.github.io/hearingvault-privacy-policy/`.
It still serves an outdated policy, so either refresh it with the same files or retire it — two
different policies online is an easy review failure.

## app-ads.txt

AdMob checks the file at the **root domain** of the developer website listed on Google Play. For
this setup that is:

```
https://devd32033-gif.github.io/app-ads.txt
```

That file is already correct:

```
google.com, pub-2698531881286039, DIRECT, f08c47fec0942fa0
```

The copy inside `/hearingvault/` is kept in sync as well. `pub-2698531881286039` is the publisher
ID behind the app ID `ca-app-pub-2698531881286039~2437237905`.

## Play Console values

- Privacy policy URL → `https://devd32033-gif.github.io/hearingvault/privacy-policy.html`
- Data deletion URL → `https://devd32033-gif.github.io/hearingvault/delete-account.html`
- Developer website → `https://devd32033-gif.github.io/hearingvault/`
- Contact email → `aacrazyenterprises@gmail.com`

All four pages are plain static HTML with no external fonts, scripts or trackers.
