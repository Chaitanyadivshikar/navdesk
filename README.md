The NAV Desk

Live site: https://chaitanyadivshikar.github.io/navdesk/

An interactive daily NAV engine that rebuilds a fund's official price the way a fund administrator's system does. Single self-contained HTML page — no frameworks, no build step.

What it computes

Only raw inputs are editable (quantities, prices, FX rates, fee terms, capital orders). Everything else is derived live:

Market values — quantity × price × FX, across a multi-currency book (USD, EUR, GBP equities + a US Treasury quoted per 100 of face)
Accrued interest — face × coupon × days ÷ 365
Fees — management fee from GAV × rate × unpaid days; performance fee only above the high-water mark
Shares outstanding — subscriptions/redemptions dealt at prior-day official NAV
Swing pricing — official price swings when net flows breach the threshold
Controls — live audit trail plus pre-release checks: bps tolerance test, positive-NAV, liability ratio, HWM logic

Conventions are simplified for demonstration (ACT/365, single share class). Figures are illustrative only.



Author

Chaitanya Divshikar — MS Finance, Simon Business School (Dec 2026) · ex-CITCO fund operations (reconciliation & NAV) · LinkedIn
