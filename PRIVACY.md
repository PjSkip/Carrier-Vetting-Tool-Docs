# Privacy Policy - Carrier Vetting Tool in Gmail (Highway.com and Carrier411)

Last updated: October 1, 2026

This policy applies to the **Carrier Vetting Tool in Gmail (Highway.com and Carrier411)** Chrome extension (Chrome Web Store item `hpejmgmlnjcfjccehkdgnjgdafmfjjao`) and the matching Tampermonkey userscript `GmailHighwayCarrier411MCBadges.user.js` (version 2026.39.4.1) published at [PjSkip/TamperMonkeyScripts](https://github.com/PjSkip/TamperMonkeyScripts).

Contact: [prostovanka@gmail.com](mailto:prostovanka@gmail.com)

## Single purpose

The tool finds MC numbers in Gmail and shows Highway and Carrier411 carrier-vetting details next to them so you can check a carrier without leaving the inbox.

## Data the tool handles

The tool runs in your browser. It does **not** operate a developer backend that receives your Gmail, Highway, or Carrier411 data. There is no paywall, Stripe, or payment processing in the tool.

### Gmail (personal communications and website content)

On `mail.google.com` (and legacy `inbox.google.com`), the tool reads the **open email / thread** only: subject, visible body text, and sender/from addresses. It does this to:

- find MC numbers (for example `MC 123456`)
- compare the sender email with Highway carrier contact emails (the Email match badge)
- draw badges and the results bar (pass/fail, power units, safety, insurance, FreightGuard, email match, copy helpers, and settings you turn on)

It does not read your whole mailbox, send email contents to the developer, or upload messages to a server we control.

### Highway and Carrier411 (website content)

The tool requests carrier records from `highway.com` and `carrier411.com` **using your existing signed-in Chrome session**. You must already be logged in. Lookups use the MC (and related identifiers) found in the email. Responses are used only to paint badges and the results bar, and to keep sessions and claims in sync when the tool also runs on Highway broker pages and Carrier411 pages.

Typical network destinations include:

- Highway monitor APIs and carrier search (for example `highway.com/monitor/api/v1/...` and Highway broker carrier search)
- Carrier411 My Carriers and company detail pages
- Highway and Carrier411 login URLs when a session needs to be established

Highway and Carrier411 are independent services. Their own privacy policies apply to your accounts with them. This tool is not made by, and is not affiliated with, Highway, Carrier411, or Google.

### Clipboard

If you click Copy on a carrier name, MC, DOT, or related helper text, the tool writes that text to the clipboard. It does not read the clipboard.

### Local storage

Using Chrome / userscript storage, the tool saves:

- your Settings (which fields are on, field order, bar vs badges layout, and similar preferences)
- a **same-day local cache** of lookup results so the same MC is not fetched again while you work
- session / claim sync flags used with Highway and Carrier411 tabs

This data stays on your computer. Uninstalling the extension or clearing site/extension data in Chrome removes it. It is not synced to a server we operate.

### Personally identifiable information

The only personal identifiers the tool handles are **email addresses already present in the open Gmail message** (typically the From address, and emails in that same message). Those addresses are used only for the Email match badge against Highway contact emails. They are not collected into a developer database.

## What we do not do

- We do not sell or transfer user data to third parties for advertising, analytics products, or credit/lending decisions.
- We do not use user data for purposes unrelated to showing carrier-vetting badges and results in Gmail.
- We do not collect passwords. Highway and Carrier411 cookies stay in your browser session with those sites.
- We do not inject remote JavaScript. Extension code ships in the Chrome Web Store package (and the matching userscript from the TamperMonkeyScripts repository).
- We do not process payments or run a paywall inside this tool.

## Sharing

The only network requests the tool makes (other than loading itself from Chrome or the userscript host) are to Highway and Carrier411 so it can display your already-authorized carrier data and keep those sessions/claims in sync. No other third parties receive Gmail or carrier data from this tool.

## Changes

If data practices change, this file will be updated and the date at the top will change.
