# BD FLIX Admin v1

## Files
- `index.html`: public catalogue; reads published titles from Supabase
- `admin.html`: admin login and movie/title manager
- `supabase-config.js`: Supabase Project URL + Publishable/anon key
- `vercel.json`: maps `/admin` to `admin.html`

## Configure
Edit `supabase-config.js` and replace the two `PASTE_...` values using Supabase Project Settings → API Keys / Connect:
- Project URL
- Publishable key (`sb_publishable_...`) or legacy anon public key

Never put a `service_role` or Secret key in browser code or GitHub.

## Admin password
Your confirmed Auth user must be present in `public.admin_users`. Open `/admin`, use Forgot password? and follow the recovery email to set a password. Supabase Auth URL Configuration should have Site URL `https://bdflix2026.vercel.app` and Redirect URL `https://bdflix2026.vercel.app/**`.

## Deploy from Android
In GitHub repository `Isfahan1202/BD-FLIX`, upload/replace these files at repository root:
`index.html`, `admin.html`, `supabase-config.js`, `vercel.json`.
Commit to `main`; Vercel will redeploy automatically.

Open:
- https://bdflix2026.vercel.app/
- https://bdflix2026.vercel.app/admin

This version supports movie/title add, edit, delete and publish/unpublish. Season/episode management and image storage uploads can be added in a later version. Only list/stream media you own or are authorized to use.
