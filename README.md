# OnlyMoney Support

Public static support and privacy website for OnlyMoney.

## Published routes

- `/` — product overview
- `/support/` — canonical English support page
- `/privacy/` — canonical English Privacy Policy
- `/en/`, `/ru/`, `/es/`, and `/de/` route prefixes — localized support and privacy content

## Publishing with GitHub Pages

1. Create a public repository named `onlymoney-support` under the `talencote` GitHub account.
2. Upload the contents of this directory to the repository root.
3. In **Settings → Pages**, select **Deploy from a branch**, branch `main`, folder `/ (root)`.
4. Wait for `https://talencote.github.io/onlymoney-support/` to become available.
5. Verify `/support/` and `/privacy/` before entering them in App Store Connect.

The site uses plain HTML and CSS. It has no analytics, cookies, forms, remote fonts, or third-party scripts.
