# MOG Cream — Shopify Theme

A custom Shopify theme for MOG Cream, built in the style of based.com. Dark, masculine, high-converting.

---

## 🚀 How to Deploy to Shopify via GitHub

### Step 1 — Push this repo to GitHub

1. Create a new repo on [github.com](https://github.com/new)
   - Name it: `mog-cream-theme`
   - Set it to **Private**
2. Open your terminal and run:

```bash
git init
git add .
git commit -m "Initial MOG Cream theme"
git remote add origin https://github.com/YOUR_USERNAME/mog-cream-theme.git
git push -u origin main
```

---

### Step 2 — Connect GitHub to Shopify

1. In your Shopify admin, go to **Online Store → Themes**
2. Click **Add theme → Connect from GitHub**
3. Authorize Shopify to access your GitHub
4. Select your `mog-cream-theme` repo and the `main` branch
5. Click **Connect**

---

### Step 3 — Upload your images

Shopify doesn't serve files directly from GitHub — images need to be in the **Files** section:

1. Go to **Content → Files** in Shopify admin
2. Upload both images:
   - `product-shot.jpg`
   - `infographic.jpg`
3. Copy the URLs Shopify gives you
4. In the Theme Editor, open **Hero** and **Infographic** sections and paste the image URLs (or use the image picker to re-upload)

---

### Step 4 — Publish the theme

1. Go to **Online Store → Themes**
2. Find **MOG Cream** in your theme list
3. Click **Publish**

---

## 🎨 Customizing in the Theme Editor

Go to **Online Store → Themes → Customize** to edit:

| Section | What you can change |
|---|---|
| Announcement Bar | Promo text |
| Header | Nav CTA label + link |
| Hero | Headline, price, product image, stats |
| Trust Bar | Icons and trust messages |
| Benefits | Cards (icon, title, description) |
| Infographic | Image |
| Ingredients | Each ingredient name + description |
| Results | Stats (number, label, description) |
| How To Use | Step title + description |
| Reviews | Reviewer name + review text |
| CTA Banner | Headline, body, button |
| Footer | Tagline, links |

---

## 🛒 Connecting to your Shopify product

1. In the Hero section, set the **CTA URL** to your product's Shopify URL (e.g. `/products/mog-cream`)
2. Repeat for the CTA Banner section
3. This way the "Add to Cart" button goes straight to checkout

---

## 📁 File Structure

```
mog-cream-theme/
├── assets/
│   ├── theme.css          # All styles
│   ├── theme.js           # Smooth scroll + nav
│   ├── product-shot.jpg   # Product image
│   └── infographic.jpg    # Benefits infographic
├── config/
│   ├── settings_schema.json
│   └── settings_data.json
├── layout/
│   └── theme.liquid       # Main HTML wrapper
├── locales/
│   └── en.default.json
├── sections/
│   ├── announcement-bar.liquid
│   ├── header.liquid
│   ├── hero.liquid
│   ├── trust-bar.liquid
│   ├── benefits.liquid
│   ├── infographic.liquid
│   ├── ingredients.liquid
│   ├── results.liquid
│   ├── how-to-use.liquid
│   ├── reviews.liquid
│   ├── cta-banner.liquid
│   └── footer.liquid
└── templates/
    └── index.liquid       # Homepage layout
```
