# DEPLOY — Path B
## 1. GitHub
git init; git add .; git commit -m "feat: NagpurAI Full Autopilot B"; git branch -M main; git remote add origin https://github.com/<YOUR-USERNAME>/nagpurai-autopilot.git; git push -u origin main
## 2. Supabase
Create project -> SQL Editor -> paste supabase/schema.sql -> Run
## 3. Vercel
New Project -> Import GitHub repo -> Add env vars -> Deploy
Preview = staging, Production = nagpurailabs.in (add domain in Vercel -> Domains)
## 4. Cloudflare (recommended)
Add domain, proxy on, SSL Full Strict, Cache rule for /_next/static
## 5. Approve Gate
Agents work on branch agent/* -> PR -> CI passes -> Vercel Preview -> YOU approve -> merge to main -> prod
