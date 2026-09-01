# KeySuite V4.21.04 Upgrade

Apply these files over V4.21.03.

Changes:
- Dashboard Brand / Series Settings has a Brand-level checkbox. Tick the Brand to tick all currently visible/eligible series under it; untick to clear all. Partial series selection shows the Brand checkbox as indeterminate.
- V4.21.03 eligibility filtering is preserved: no customer = User Assigned only; customer selected = User Assigned × Customer Price Preference.
- CHC C4 (G1) Enhanced is available again, but defaults unticked.
- Dashboard Quick Selection supports Enhanced independently for CHC C4 and CHC C6, and saves the Enhanced preference per CHC series/generation.
- C4 continues to use G1 hydraulic data and IE2 motor defaults.

Deployment:
- Replace/upload the web files.
- No Supabase db push required.
- No Edge Function deploy required.
