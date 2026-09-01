# V4.21.10 Upgrade

Replace the included web-app files and Supabase function files, then redeploy:

```powershell
npx.cmd supabase@latest functions deploy telegram-webhook --no-verify-jwt
```

No `supabase db push` is required for V4.21.10.
