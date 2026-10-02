# Privacy Policy - Carrier Vetting Tool in Gmail (Highway.com and Carrier411)

Last updated: October 1, 2026

This privacy policy applies to **Carrier Vetting Tool in Gmail (Highway.com and Carrier411)** (Chrome Web Store item ID `hpejmgmlnjcfjccehkdgnjgdafmfjjao`) and the matching Tampermonkey userscript `GmailHighwayCarrier411MCBadges.user.js` version 2026.39.4.1 (October 1, 2026) in [PjSkip/TamperMonkeyScripts](https://github.com/PjSkip/TamperMonkeyScripts).

Contact: [prostovanka@gmail.com](mailto:prostovanka@gmail.com)

## Single purpose

Scan open Gmail threads for MC numbers and display Highway and Carrier411 carrier-vetting results (results bar / badges) so you can check a carrier without leaving Gmail. Settings are available from the truck icon. The same tool also runs on Highway and Carrier411 pages to keep login sessions and claims in sync.

## What data is read

### In Gmail

On `mail.google.com` (and legacy `inbox.google.com`), the tool reads the **currently open email or thread only**: subject, visible body text, and sender / from addresses. It uses that content to:

- find MC numbers
- compare sender email with Highway carrier contact emails (email match)
- draw the results bar / badges (pass/fail, power units, safety, identity alerts, Do Not Use, email match, FreightGuard, freight loss, and other fields you enable)

It does **not** read your whole mailbox and does **not** upload Gmail contents to a developer-operated server.

### On Highway and Carrier411

Using your existing signed-in Chrome sessions, the tool requests carrier records from Highway and Carrier411 for MCs found in Gmail (and related sync work on those sites). You must already be logged in to those services.

## Where data is sent

Network requests go **only** to:

- Highway (`highway.com`), including broker UI, login, carrier search, and monitor APIs
- Carrier411 (`carrier411.com` / `www.carrier411.com`), including My Carriers, company detail, and login

No other third-party analytics, advertising, payment, or developer backend receives Gmail or carrier data from this tool. There is **no Stripe** and **no paywall** in the product.

Highway and Carrier411 are independent services with their own privacy policies. This tool is not made by and is not affiliated with Highway, Carrier411, or Google.

## Local storage (stays on your device)

The tool stores on your computer (Chrome / userscript storage):

- Settings (fields shown, layout, and related preferences from the truck icon)
- A same-day local cache of lookup results
- Session / claim sync flags used with Highway and Carrier411 tabs

This data is not synced to a ShipSierra server. Clearing extension or site data, or uninstalling, removes it.

## Clipboard

Copy helpers may write carrier name, MC, DOT, or related text to the clipboard when you click Copy. The tool does not read the clipboard.

## Personally identifiable information

The only personal identifiers handled are email addresses **already present in the open Gmail message** (typically From, and emails in that same message), used only for the email match badge against Highway contacts. They are not collected into a developer database.

## What we do not do

- We do not sell or transfer user data to third parties for advertising, analytics products, or credit / lending decisions
- We do not use user data for purposes unrelated to carrier vetting in Gmail
- We do not collect passwords (Highway and Carrier411 cookies stay with those sites)
- We do not inject remote JavaScript; code ships in the Chrome Web Store package and the TamperMonkeyScripts userscript
- We do not process payments or run a paywall

## Changes

If practices change, this file will be updated and the date at the top will change.
