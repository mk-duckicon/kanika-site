# KANIKA — Vercel Deploy (GoDaddy domain)

## 1) Deploy to Vercel
- Go to https://vercel.com → Add New Project → Import
- Drag the contents of this folder (index.html, logo.png, favicon.png)
- Framework = "Other" (or No framework)
- Deploy → you get a temporary vercel.app URL

## 2) Connect your domain (getkanika.com)
In Vercel → Project → Settings → Domains → Add → getkanika.com

In GoDaddy DNS for getkanika.com add:
- A  @  76.76.21.21
- CNAME  www  cname.vercel-dns.com

Wait a few minutes; Vercel will verify and issue SSL.

## 3) Redirect kanika.ai → getkanika.com
Option A (GoDaddy Forwarding): Domain → Forwarding → Add → Permanent (301) to https://getkanika.com  
Option B (Vercel): Add kanika.ai in Domains → set as Redirect to getkanika.com

## 4) Email (Google Workspace)
Add alias info@getkanika.com in Admin Console → Users → (you) → Email aliases.
Then in Gmail: Settings → Accounts → "Send mail as" → add info@getkanika.com.

You're live!
