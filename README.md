# KeySuite V4.21.12 UPGRADE

Full-clean continuation built from the verified KeySuite V4.20.01 baseline.

## CHC impeller adjustment

- Custom reduced/small impeller counts now use the visible CHC suffix instead of `(Custom)`.
- Example: CHC 32-30 with 3 small/reduced impellers displays as `CHC 32-30-3`.
- Example: CHC 32-80 with 5 small/reduced impellers displays as `CHC 32-80-5`.
- Pricing remains tied to a valid catalog SKU. When the custom reduced count is beyond the catalog range, pricing uses the closest available reduced-impeller SKU for the same base model.
- Therefore CHC 32-30-3 prices from CHC 32-30-2, and CHC 32-80-5 prices from CHC 32-80-2.
- Existing exact catalog impeller models continue to use their exact model name and price.
- Existing physical `Reduce Impeller` stage-removal behavior remains unchanged.

## V4.20.01 pricing correction retained

- Fixed Price remains global/customer-independent.
- Fixed rows are resolved before customer Pricing Category currency filters.
- Fixed pricing does not require USD/RMB/MYR to be selected.
- Fixed pricing continues to bypass margin, rarity factors, transport, discounts, fuel charge, and RM10 rounding.

No SQL migration is required.


## V4.21.02 CHC G1
See `README_V42102.md` for the G1 hydraulic and V1.1 price-model changes.


## V4.21.03 Dashboard Brand / Series
See `README_V42103.md` for the Dashboard no-customer User Assigned behavior and customer intersection rule.


## V4.21.04 Brand checkbox + C4 Enhanced
See `README_V42104.md` for Brand-level select-all behavior and C4 Enhanced availability/default.


## V4.21.05 C4/G1 PDF dimensions
See `README_V42105.md` for the corrected C4/G1 dimension drawings and G1 numeric dimension table used by PDF export.


## V4.21.07
See `README_V42107.md` for the PDF metadata, Quick Selection first-click, Dashboard Item reset and PDC changes.


## V4.21.08
See `README_V42108.md` for the corrected independent PDC checkbox and quotation payment-term formatting.


## V4.21.09
See `README_V42109.md` for the CHC G1/G2 admin Price Group and C4/C6 user-facing naming normalization.


## V4.21.10
- KeyBot guided model buttons no longer fall into global duplicate matching.
- Hi / New Request / Back escape pending Brand / Model choice state.
- Unscoped B.G.Reich CHC ambiguity is labelled C4/C6.

## V4.21.11
Rebuilt from V4.21.10. Cache token is `42111`. Deploy `telegram-webhook`; no database push is required.

## V4.21.12
KeyBot / Telegram CHC C4 PDF Page 3 now uses the correct G1 dimension drawing assets. C6/G2 is unchanged. No database push is required; redeploy `telegram-webhook`.
