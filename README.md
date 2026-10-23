# OnlyMoney Support

Public static support and privacy website for OnlyMoney.

## Published routes

- `/` — product overview
- `/support/` — canonical English support page
- `/privacy/` — canonical English Privacy Policy
- `/support/apple-pay/` and `/en/support/apple-pay/`, `/ru/support/apple-pay/`, `/es/support/apple-pay/`, `/de/support/apple-pay/` — Apple Pay automation setup guides
- `/en/`, `/ru/`, `/es/`, and `/de/` route prefixes — localized support and privacy content

## Publishing with GitHub Pages

1. Create a public repository named `onlymoney-support` under the `talencote` GitHub account.
2. Upload the contents of this directory to the repository root.
3. In **Settings → Pages**, select **Deploy from a branch**, branch `main`, folder `/ (root)`.
4. Wait for `https://talencote.github.io/onlymoney-support/` to become available.
5. Verify `/support/` and `/privacy/` before entering them in App Store Connect.

The site uses plain HTML and CSS. It has no analytics, cookies, forms, remote fonts, or third-party scripts.

## Apple Pay guide maintenance

The guide describes the OnlyMoney Record Apple Pay Expense action: an explicit
active account, a currency-bearing amount, optional merchant, and the protected
Other Expenses category. Keep action labels and category translations synchronized
with the application. The guide uses numbered instructions and a field mapping table, without decorative
flow tiles or simulated iOS screenshots. Add genuine privacy-safe screenshots after physical-device setup
verification; never include real card, account, or purchase details.

The optional automation stores payment data locally. The prepared Privacy Policy
update explains this input source and user control of the automation. Publish the
guide, FAQ, privacy, and sitemap changes in the same release cycle. Local edits
are not a deployment. After publication, verify every guide language route and
the updated canonical policy over HTTPS.
