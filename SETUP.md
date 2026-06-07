# Fumi DFW Realtor — Setup & Deploy Guide

## 1. ADD YOUR IMAGES
Place these files in the `images/` folder:
- `hero.jpg`         — hero background (kitchen/modern interior from Canva)
- `fumi-photo.jpg`   — Fumi's portrait photo
- `listing-1.jpg`    — mixed-use property photo
- `listing-2.jpg`    — suburban home photo
- `listing-3.jpg`    — apartment photo
- `service-buying.jpg`  — buying service card background
- `service-selling.jpg` — selling service card background
- `service-rental.jpg`  — rental service card background

Export each from Canva: select the image → right-click → Save image as → save to images/

## 2. GET YOUR WEB3FORMS KEY (contact form, FREE)
1. Go to https://web3forms.com
2. Enter: FUMI@FUMIDFWREALTOR.COM → click "Create Access Key"
3. Copy the key
4. Open index.html → find: YOUR_WEB3FORMS_KEY_HERE → replace with your key

## 3. ADD YOUR INSTAGRAM HANDLE
Open index.html → find: YOUR_INSTAGRAM_HANDLE → replace with handle (no @)
Example: https://www.instagram.com/fumidfwrealtor

## 4. PUSH TO GITHUB
1. Create a new repo at github.com (name: fumi-dfw-realtor, Public)
2. Run:
   git init
   git add .
   git commit -m "Initial site"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/fumi-dfw-realtor.git
   git push -u origin main

## 5. DEPLOY ON CLOUDFLARE PAGES
1. Go to https://dash.cloudflare.com → Pages → Create a project
2. Connect to Git → select your fumi-dfw-realtor repo
3. Build settings: leave blank (static HTML, no build needed)
4. Deploy → Cloudflare gives you a free URL (e.g. fumi-dfw-realtor.pages.dev)

## 6. CONNECT YOUR DOMAIN (luxfrills.com)
Since your domain is already on Cloudflare:
1. In Cloudflare Pages → your project → Custom Domains
2. Add: luxfrills.com
3. Cloudflare connects it automatically (no DNS config needed)
4. SSL is automatic and free

## DONE ✓
Your site will be live at https://luxfrills.com
