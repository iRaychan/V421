# KeySuite V4.21.13 UPGRADE

This upgrade continues V4.21.12 and includes the V4.21.13 fixes.

- KeyBot CHC C4/G1 PDF Page 3 dimension drawings are loaded from `assets/chc-g1-dimensions/` instead of being embedded in the Edge Function bundle.
- KeyPLC Price List adds missing `3kW` and `37kW` rows.
- Run `V42113_KEYPLC_3KW_37KW_SQL_EDITOR.sql` (or the timestamped migration) and redeploy `telegram-webhook`.

See `README_V42113.md`.
