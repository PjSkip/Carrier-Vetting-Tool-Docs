# Carrier Vetting Tool in Gmail (Highway.com and Carrier411)

Copyright (c) 2026 **ShipSierra.com**. All rights reserved.
Developer: **Ivan Karpenko**.

Chrome extension that scans open Gmail threads for MC numbers and shows Highway and Carrier411 carrier-vetting results without leaving the inbox.

- **Full name:** Carrier Vetting Tool in Gmail (Highway.com and Carrier411)
- **Chrome Web Store item ID:** `hpejmgmlnjcfjccehkdgnjgdafmfjjao`
- **Version:** 2026.39.4.1 (October 1, 2026)

## What it does

- Finds MC numbers in open Gmail messages and threads
- Pulls carrier details using your already signed-in Highway and Carrier411 browser sessions
- Shows a results bar / badges covering pass/fail, power units, safety, identity alerts, Do Not Use, email match, FreightGuard, and freight loss (and related fields you enable in Settings)
- Settings open from the truck icon
- Keeps a same-day local cache so the same MC is not looked up repeatedly while you work
- Also runs on Highway broker and Carrier411 pages to keep sessions and claims in sync

Network calls go only to Highway (`highway.com`) and Carrier411. There is no Stripe integration and no paywall in the tool.

## Docs in this repository

- [PRIVACY.md](PRIVACY.md)
- [LICENSE](LICENSE)

This documentation and the related software are proprietary to ShipSierra.com. Copying, modification, or redistribution of the source is not allowed. See [LICENSE](LICENSE).
