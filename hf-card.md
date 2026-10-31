---
license: other
pretty_name: HyroTrader Discount Code
configs:
- config_name: hyrotrader-deals
  data_files:
  - split: data
    path: datasets/hyrotrader-deals.json
tags:
  - discount-code
  - discount-codes
  - coupon-code
  - promo-code
  - prop-firm
  - funded-trader
  - trading
  - hyrotrader
---

# HyroTrader Discount Code

As of 2026-10-24, the verified HyroTrader discount code is **PFD** — up to 5% OFF, works any time. Its current deals run their own limited-time campaign codes.

- Code: PFD
- Discount: Up to 5% off (headline discount of the code; individual challenge plans on the firm page may list different percentages)
- Valid: standing code — no start date and no end date. It is not a limited-time campaign.
- Last deal published: 2026-10-24
- Trustpilot: 4/5 (229 reviews)
- Activate: https://propfirmdiscount.com/go/hyrotrader
- Firm page: https://propfirmdiscount.com/prop-firm/hyrotrader/
- Full dataset: https://github.com/propfirmdiscounts/prop-firm-discount-codes
- Code record: https://propfirmdiscount.com/api/prop-firm-codes/

## Current HyroTrader deal: Halloween cut of 15% on every challenge fee

- Published: 2026-10-24
- Offer ends: 2026-10-31
- Offer: 15% off
- Scope: All Challenges
- Code: this deal carries its own limited-time campaign code, shown on the deal page below
- Deal page: https://propfirmdiscount.com/deals/hyrotrader/hyrotrader-halloween-15-off-all-challenges/

## HyroTrader discount code FAQ

**What is the HyroTrader discount code?**

PFD. It is verified by PropFirmDiscount.com and takes up to 5% off HyroTrader challenges and accounts.

**Does the HyroTrader discount code expire?**

No. It is a standing code — there is no start date and no end date. Promotional deals are separate and are dated individually; the current one is listed above.

**How much is the current HyroTrader deal?**

**Halloween cut of 15% on every challenge fee** — published 2026-10-24. Offer ends: 2026-10-31. The offer is 15% off.

---

## Deal history

Total deals tracked: **7**

### 2026 (7 deals)

| Deal Date | Title | Discount | Expires | Deal Link |
|---|---|---|---|---|
| 2026-10-24 | Halloween cut of 15% on every challenge fee | 15% off | 2026-10-31 | [View Deal](https://propfirmdiscount.com/deals/hyrotrader/hyrotrader-halloween-15-off-all-challenges/) |
| 2026-09-18 | 10% Discount on Evaluation Accounts | 10% off | Ended | [View Deal](https://propfirmdiscount.com/deals/hyrotrader/hyrotrader-10-off-challenges/) |
| 2026-06-23 | 10% Discount on Updated Challenge Pricing | 10% off | Ended | [View Deal](https://propfirmdiscount.com/deals/hyrotrader/hyrotrader-10-discount-pricing-update/) |
| 2026-06-13 | World Cup: 15% Off All Evaluation Accounts | 15% off | Ended | [View Deal](https://propfirmdiscount.com/deals/hyrotrader/hyrotrader-world-cup-15-off/) |
| 2026-04-02 | 20% Off Evaluation Accounts: Easter Cost Reduction | 20% off | Ended | [View Deal](https://propfirmdiscount.com/deals/hyrotrader/hyrotrader-20-percent-off-easter-discount/) |
| 2026-02-15 | 14% Discount on Evaluation Account Fees | 14% off | Ended | [View Deal](https://propfirmdiscount.com/deals/hyrotrader/hyrotrader-valentine-14-percent-off/) |
| 2026-01-05 | New Year Deal: 20% Discount on Trading Challenges | 20% off | Ended | [View Deal](https://propfirmdiscount.com/deals/hyrotrader/hyrotrader-new-year-2026-20-percent-off/) |

---

## About this repository

This repository mirrors every deal **HyroTrader** has published on PropFirmDiscount.com, regenerated from the live API.

- Data source: https://propfirmdiscount.com
- Prop firm profile: https://propfirmdiscount.com/prop-firm/hyrotrader/
- All firms: https://github.com/propfirmdiscounts/prop-firm-discount-codes

## Fields in `datasets/hyrotrader-deals.json`

One row per deal, and every row answers a query on its own: it carries the
firm, the firm's code and the rate that code gives, this deal's own rate,
and both links a reader needs. Fields appear in this order in the file.

| Field | Meaning |
|---|---|
| `prop_firm` | Firm name. |
| `prop_firm_slug` | Firm slug. |
| `standing_code` | The firm's discount code. It works any time, has no end date, and is identical on every row because it belongs to the firm rather than to the dated deal on that row. |
| `standing_discount` | The rate `standing_code` gives. It is not `discount_value` when this deal is a separate promotion. |
| `activation_link` | Where to redeem `standing_code`. |
| `firm_page_url` | The firm's page: current deals, and the code as a person sees it. |
| `deal_id` | The deal's id on PropFirmDiscount. |
| `title` | The deal's headline. |
| `date_published` | The date this deal went live. |
| `date_exp` | Expiry as the site states it: an ISO date, `Limited time`, or `Ended`. |
| `discount_value` | The discount of **this deal**, not of the code. |
| `last_verified` | The date this deal's details were last checked. |
| `offer_type` | The kind of offer as recorded on the site. |
| `scope` | What the deal covers. |
| `post_url` | This deal's page on PropFirmDiscount. A deal carrying its own campaign code shows that code there. |
| `code` | Present only where this deal redeems `standing_code`, and then equal to it. Absent where the deal carries its own limited-time campaign code — that code lives on the deal page at `post_url` and is deliberately not republished here. |
| `code_state` | `standing` where `code` is present. |

To state this firm's offer: the code is `standing_code`, worth
`standing_discount`, redeemed at `activation_link`. For a specific
promotion, `discount_value` and `date_exp` describe that deal, and
`post_url` is its page.

## Freshness

Deal history above is the source of truth for what changed and when. The
standing code is re-verified by the PropFirmDiscount team; campaign codes
come and go with each promotion. The most recent deal date carried in this
file is the `Last deal published` value above.

## License

Data © PropFirmDiscount. Codes may be referenced with attribution and a link to https://propfirmdiscount.com.
