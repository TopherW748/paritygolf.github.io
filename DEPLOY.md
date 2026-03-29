# Deploying to GitHub Pages

## Step 1 — Add the icon
Copy your Looper Golf app icon image into `assets/looper-icon.png`.
(Any reasonable resolution works — 512x512 is ideal.)

## Step 2 — Create a new GitHub repository
- Go to github.com → New repository
- Name it: `paritygolf.github.io`  ← this gives you a free URL at that address
  OR any name (e.g. `looper-website`) — you'll get `paritygolf.github.io/looper-website`
- Set it to Public
- Don't add a README

## Step 3 — Push these files
```bash
cd website/
git init
git add .
git commit -m "Initial website"
git branch -M main
git remote add origin https://github.com/paritygolf/paritygolf.github.io.git
git push -u origin main
```

## Step 4 — Enable GitHub Pages
- In the repo → Settings → Pages
- Source: Deploy from branch → main → / (root)
- Save

Your site will be live at: https://paritygolf.github.io (or your repo URL) within ~2 minutes.

## Step 5 — Custom domain (optional, ~$12/year)
1. Buy a domain (e.g. `loopergolf.app` or `paritygolf.se`) from Namecheap / Cloudflare
2. In GitHub Pages settings → Custom domain → enter your domain
3. Add a CNAME DNS record at your registrar pointing to `paritygolf.github.io`

## What to use in App Store Connect
- **App URL / Marketing URL:** your GitHub Pages URL
- **Privacy Policy URL:** `https://paritygolf.github.io/privacy.html`
- **Support URL:** `mailto:paritygolfab@gmail.com` or the main site URL
