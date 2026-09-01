# KeySuite V4.21.10

KeyBot exact-model context-lock fix.

- Product path keeps selected Brand and C4/C6 generation locked through exact model selection.
- Selecting an exact CHC C4/C6 or ES model opens it directly and generates the rated curve on the same click.
- Global exact-model disambiguation is used only when the request is actually outside a scoped Product catalogue choice.
- Ambiguous direct CHC searches identify C4/C6 in the choice label so two generations never appear as identical B.G.Reich buttons.
- No Supabase database migration. Redeploy `telegram-webhook`.
