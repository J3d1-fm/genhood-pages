# Changelog

## 0.1.11 - 2026-11-24

- Privacy policy: the player profile is backed up through PurchaseKit under the player ID, and the backup includes the house, the empire name and saved conversations with the in-game creators, including replies the player selects or types.
- Removed the statement that what the player picks or types in chats is not sent to us; added that chats use scripted dialogue and that on supported devices an on-device model can answer typed text, with replies generated on the device.
- PurchaseKit is now described as the game-save and purchase-verification service in the data and partner sections.
- Rollback: revert this commit to return to 0.1.10. Do not roll back while an Android build that backs up conversations is available in Google Play.

## 0.1.10 - 2026-11-24

- Added the Terms of Service for Bloghouse Rivals on Android at /terms-of-service.
- Linked the terms from the home, careers and privacy pages and added the address to the sitemap.

## 0.1.9 - 2026-11-24

- Privacy policy updated for the Android release of Bloghouse Rivals with ads (1.5.22, build 149): rewarded video, a menu banner and sponsored cards after the first sessions (none for players who have purchased), no full-screen ads between screens.
- Disclosed Google AdMob: the advertising ID and ad-request data, Google's consent form in the EEA, the UK and Switzerland (no ad requests before an answer, non-personalised ads without consent), the opt-out for US states, privacy options in the Game's settings, device ad settings elsewhere.
- Replaced "no ads, no advertising ID" and "we do not share data for cross-app advertising" with what the build does. Firebase Analytics still receives no advertising ID (checked in the build's manifest).
- Rollback: revert this commit to return to 0.1.8. Do not roll back while a build with ads is available in Google Play.

## 0.1.8 - 2026-10-22

- Rewrote the privacy policy for Bloghouse Rivals on Android to match what the game does: no account and device-stored progress, Unity Gaming Services anonymous player ID, PurchaseKit purchase verification and offer events, Firebase Analytics without advertising ID, no ads, Meta component switched off (earlier versions disclosed), deletion by email within one month, 13+.
- Removed statements the game does not support: an in-game "Delete my account" button, sign-in via email/Facebook/Apple/Google/Huawei, AppMetrica, a data protection officer approval step, "low-level formatting" and NaCl encryption claims, the summer 2026 App Store date.
- The iOS version is published by Eponymical Games Ltd; the page links its policy.
- Rollback: revert this commit to return to 0.1.7.

## 0.1.7 - 2026-09-29

- Added a homepage News section with three friendly development updates and Google Play invitations.
- Distinguished the live Android game from welcome/reward improvements under testing and the upcoming iOS version.
- Added News navigation in the header and footer, responsive cards and keyboard focus styling.
- Recorded source provenance and rollback instructions in the technical documentation.

## 0.1.6 - 2026-09-28

- Updated the homepage, social preview and platform summary for the current Bloghouse Rivals release.
- Made the verified Google Play download link prominent in the hero and game section.
- Replaced the outdated summer App Store promise with iOS in development, without a launch date or placeholder store link.
- Replaced the unsupported aspirational 100M+ counter with the debut game name and aligned the game description with the public listing.

## 0.1.5 - 2026-07-02

- Added the Search Console URL-prefix property `https://www.genhood.com/` under the project-bound Google account `ceo@genhood.com`.
- Confirmed the URL-prefix property through the existing DNS provider verification instead of an HTML file.
- Documented that both `genhood.com` domain property and `https://www.genhood.com/` URL-prefix property are owned by `ceo@genhood.com`.

## 0.1.4 - 2026-07-02

- Removed the `googleac09d6a6592613bd.html` URL-prefix verification file that was created under the wrong Google organization account.
- Switched Search Console ownership handling to the existing DNS-based domain verification for `genhood.com` under `ceo@genhood.com`.
- Updated technical documentation to record the corrected account-routing rule and rollback point.

## 0.1.3 - 2026-07-02

- Added Google Search Console HTML verification file `googleac09d6a6592613bd.html`.
- Prepared `https://www.genhood.com/` URL-prefix ownership verification for Google Play Console website ownership checks.
- Updated project technical documentation for the new root verification file and rollback point.

## 0.1.2 - 2026-07-02

- Added root `app-ads.txt` for AdMob app ownership and seller authorization checks.
- Published the AdMob line `google.com, pub-2370609296461964, DIRECT, f08c47fec0942fa0`.
- Updated project documentation for the new root file and rollback point.

## 0.1.1 - 2026-06-15

- Added `pitch/genhood_bloghouse_seed_2026_en.pdf` as the English investor deck.
- Updated `pitch.html` so the deck download button uses the English PDF for EN and the Russian PDF for RU.
- Updated `pitch/interactive.html` so all PDF deck buttons switch URLs when the active language changes.
- Regenerated the English PDF deck from the Russian PPTX template while preserving the deck layout.

## 0.1.0 - 2026-06-15

- Added an EN/RU language switcher to the confidential investor materials cover page.
- Added localized English and Russian copy for `pitch.html`.
- Preserved the selected language in `localStorage` and passed it to the interactive pitch URL.
- Added project version, changelog, and technical documentation files for rollback tracking.
