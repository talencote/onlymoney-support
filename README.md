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

## AI-assisted migration

`/support/import/` and en/ru/es/de equivalents describe user-mediated conversion
with an external AI service. `assets/onlymoney-ai-import-guide.md` is the English
provider-neutral specification; the source is `Support/onlymoney-ai-import-guide.md`
in the app repository. Update it alongside backup-format changes and regenerate
the app's synthetic compatibility fixture using `scripts/verify_import_guide.py`.
The AI must analyze first and wait for approval before generating a backup.
Keep replacement warnings, privacy disclosures, support links, and sitemap in sync.
No financial upload endpoint or AI API integration exists on this site.
Local edits are not publication; verify the guide download and every route after
deployment. Do not promise compatibility with every export or a free AI plan.

Guide revision 2 also accepts an optional current OnlyMoney backup. The AI keeps
its history and appends the export with agreed account mappings and base currency.
Duplicate investigation and exact balance reconciliation are not required;
announced opening-balance defaults and approximate conversions are covered by
one plan approval. Structural file validation remains mandatory.
