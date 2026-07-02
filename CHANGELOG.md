# Changelog

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
