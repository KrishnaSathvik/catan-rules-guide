# 🏝️ Catan Rules — The Interactive Guide

An interactive, beautifully illustrated guide to the **Catan** board game — simple enough for anyone to learn in minutes. Built as a single-page static site with pure HTML, CSS, and JavaScript.

![Catan Rules Guide](https://img.shields.io/badge/Catan-Rules%20Guide-f0c040?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI+PHBhdGggZD0iTTEyIDJMMyA3djEwbDkgNSA5LTV2LTEweiIgZmlsbD0id2hpdGUiLz48L3N2Zz4=)
![License](https://img.shields.io/badge/license-MIT-2a6b7c?style=for-the-badge)
![Deploy](https://img.shields.io/badge/deploy-Vercel-000?style=for-the-badge&logo=vercel)

---

## ✨ Features

- **9 Interactive Sections** — Overview, Setup, Your Turn, Building Costs, Trading, The Robber, Development Cards, Winning, and a Dice Tool
- **Rich SVG Illustrations** — Custom-drawn hex board, game pieces (settlements, cities, roads), resource cards, robber scenes, dev card fan, harbor trade diagrams, and VP breakdowns — all pure SVG, no external images
- **Interactive Dice Roller** — Roll animation with shake effect, running roll counter, and a 7 triggers the robber indicator
- **Probability Chart** — Visual bar chart showing dice roll distributions (why 6 and 8 are the best tiles)
- **Victory Point Tracker** — Click circles to track your VP from 1–10 with celebration message
- **Collapsible Dev Cards** — Tap to expand each of the 5 development card types with rules
- **Mobile-First Responsive** — Works perfectly on phones, tablets, and desktops
- **Zero Dependencies** — Pure HTML/CSS/JS, no frameworks, no build step
- **Sticky Navigation** — Tabbed interface with smooth scroll, always accessible

## 📸 What's Inside

| Section | Visual Highlights |
|---------|------------------|
| **Hero** | Full hex board with terrain tiles, number tokens, settlements & roads |
| **Overview** | 5 hoverable resource cards with gradient styling and terrain labels |
| **Setup** | 6 illustrated component cards, board assembly diagram, distance rule visual |
| **Your Turn** | Dice → hex → resource flow diagram, player trade & bank trade illustrations |
| **Building** | Game piece showcase (road, settlement, city, dev card) with cost grid |
| **Trading** | 3 harbor rate comparison cards (4:1, 3:1, 2:1) |
| **Robber** | Robbery scene with blocked hex, steal card illustration |
| **Dev Cards** | Fanned card spread showing all 5 types with counts |
| **Winning** | VP sources illustrated with game pieces, interactive tracker |
| **Dice Tool** | Animated roller + probability bar chart |

## 🚀 Quick Start

### Run Locally

```bash
# Clone the repo
git clone https://github.com/YOUR_USERNAME/catan-rules-guide.git
cd catan-rules-guide

# Open directly in browser
open public/index.html

# Or serve locally
npx serve public
```

### Deploy to Vercel

#### Option 1: One-Click Deploy

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/YOUR_USERNAME/catan-rules-guide)

#### Option 2: CLI Deploy

```bash
# Install Vercel CLI (if not installed)
npm i -g vercel

# Deploy from project root
cd catan-rules-guide
vercel

# For production deployment
vercel --prod
```

#### Option 3: GitHub Integration

1. Push this repo to GitHub
2. Go to [vercel.com/new](https://vercel.com/new)
3. Import your GitHub repository
4. Vercel auto-detects the `vercel.json` config
5. Click **Deploy** — done!

No build step, no environment variables, no configuration needed.

## 📁 Project Structure

```
catan-rules-guide/
├── public/
│   ├── index.html       # The entire app — single file, zero deps (SEO-optimized)
│   ├── og-image.png     # Open Graph social sharing image (1200×630)
│   ├── og-image.svg     # Source SVG for the OG image
│   ├── sitemap.xml      # XML sitemap for Google Search Console
│   └── robots.txt       # Crawler directives + sitemap reference
├── vercel.json           # Vercel config (caching, headers, security)
├── package.json          # Project metadata & scripts
├── .gitignore
├── LICENSE
└── README.md
```

## 🔍 SEO — Getting Found on Google

This project is fully SEO-optimized out of the box. Here's what's included and what you need to do after deploying:

### What's Already Built In

| SEO Feature | Status |
|---|---|
| Optimized `<title>` tag (keyword-first, 55 chars) | ✅ |
| Meta description (155 chars, action-oriented) | ✅ |
| Target keywords meta tag | ✅ |
| Canonical URL | ✅ |
| Open Graph tags (Facebook, LinkedIn, Discord) | ✅ |
| Twitter Card (large image summary) | ✅ |
| OG image (1200×630 PNG) | ✅ |
| FAQPage structured data (7 Q&As — rich results eligible) | ✅ |
| WebPage + Game schema.org markup | ✅ |
| BreadcrumbList schema | ✅ |
| XML Sitemap | ✅ |
| robots.txt | ✅ |
| Semantic HTML (`<header>`, `<main>`, `<nav>`, `<footer>`) | ✅ |
| Mobile-responsive (viewport meta) | ✅ |
| Emoji favicon | ✅ |
| Fast load (zero JS deps, inline CSS, no external calls except fonts) | ✅ |
| Security headers (via vercel.json) | ✅ |

### After Deploying — Do These 5 Things

**1. Update the canonical URL**
Replace `catan-rules-guide.vercel.app` with your actual domain in `index.html` (search for it — appears in canonical, OG, Twitter, and schema tags).

**2. Submit to Google Search Console**
- Go to [search.google.com/search-console](https://search.google.com/search-console)
- Add your site as a property
- Submit your sitemap: `https://YOUR-DOMAIN/sitemap.xml`
- Use "URL Inspection" to request indexing of your homepage

**3. Validate Structured Data**
- Test at [Google Rich Results Test](https://search.google.com/test/rich-results)
- Paste your URL — should show FAQPage, WebPage, and BreadcrumbList as valid
- FAQ rich results can appear as expandable dropdowns in Google search

**4. Submit to Bing Webmaster Tools**
- Go to [bing.com/webmasters](https://www.bing.com/webmasters)
- Add your site and submit the sitemap

**5. Build Backlinks (The Real SEO Juice)**
- Share on Reddit (r/boardgames, r/catan)
- Post on BoardGameGeek forums
- Share on X/Twitter, LinkedIn, and Facebook board game groups
- Submit to board game resource directories
- Write a Medium article linking to your guide

### Target Keywords

The page is optimized for these search terms:
- `catan rules` / `catan rules explained`
- `how to play catan`
- `catan board game rules`
- `settlers of catan rules`
- `catan beginner guide`
- `catan building costs`
- `catan robber rules`
- `catan development cards`
- `what happens when you roll a 7 in catan`

## 🎨 Design Details

- **Typography** — Crimson Pro (serif headings) + DM Sans (body) from Google Fonts
- **Color Palette** — Ocean blues (`#2a6b7c`), warm sand (`#f5e6c8`), and resource-matched colors (brick red, forest green, grain gold, ore gray, pasture lime)
- **Aesthetic** — Warm, island-themed with card-based layout, soft shadows, and subtle hover effects
- **Animations** — Tab transitions, dice shake, card expand/collapse, VP tracker fill, resource card hover lift

## 📖 Rules Source

All game rules are based on the **Catan 5th Edition** official rulebook by Klaus Teuber, cross-referenced with multiple established board game rules sources including catan.com, UltraBoardGames, BoardGameArena, and colonist.io.

> **Disclaimer:** This is an unofficial fan-made guide. CATAN is a registered trademark of Catan GmbH. This project is not affiliated with or endorsed by Catan GmbH or Catan Studio.

## 🛠️ Customization

Since it's a single HTML file, customization is straightforward:

- **Colors** — Edit the CSS variables in `:root` at the top of `index.html`
- **Content** — Each section is clearly labeled with HTML comments (`<!-- ═══ SETUP ═══ -->`)
- **Add sections** — Add a new `nav-btn` + matching `section` element; the JS handles the rest
- **SVG illustrations** — All inline, editable directly in the HTML

## 📱 Browser Support

- Chrome 80+
- Firefox 78+
- Safari 14+
- Edge 80+
- Mobile browsers (iOS Safari, Chrome Android)

## 📄 License

MIT — see [LICENSE](LICENSE) for details. Use it, fork it, share it at your next game night.

---

<p align="center">
  Made with ❤️ for board game nights<br>
  <strong>🧱 🪵 🐑 🌾 ⛏️</strong>
</p>
