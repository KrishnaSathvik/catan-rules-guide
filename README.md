# 🏝️ Catan Rules — The Interactive Guide

An interactive, beautifully illustrated guide to the **Catan** board game and its expansions — simple enough for anyone to learn in minutes. Built as a multi-page static site with pure HTML, CSS, and JavaScript.

![Catan Rules Guide](https://img.shields.io/badge/Catan-Rules%20Guide-f0c040?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI+PHBhdGggZD0iTTEyIDJMMyA3djEwbDkgNSA5LTV2LTEweiIgZmlsbD0id2hpdGUiLz48L3N2Zz4=)
![License](https://img.shields.io/badge/license-MIT-2a6b7c?style=for-the-badge)
![Deploy](https://img.shields.io/badge/deploy-Vercel-000?style=for-the-badge&logo=vercel)

---

## ✨ Features

### Guides
- **Base Game Guide** — 9 interactive sections: Overview, Setup, Your Turn, Building, Trading, Robber, Dev Cards, Winning, and Searchable Almanac
- **Seafarers Expansion Guide** — Ships, pirate, gold hexes, fog tiles, 9 scenarios, building costs, and strategy tips
- **Coming Soon** — Cities & Knights, Traders & Barbarians, Explorers & Pirates (announced via scrolling ticker on homepage)

### Map Randomizer Tool
- **Balanced Board Generator** — Generate random Catan boards for 3–4 and 5–6 player games
- **Balance Rules** — Toggle constraints: no adjacent 6/8, no adjacent same terrain, no adjacent 2/12
- **Rich Map Rendering** — Ocean water frame, terrain gradient hexes, sandy coastline border, game-like cream number tokens with drop shadows, pip dots
- **Custom SVG Terrain Icons** — Hand-crafted vector icons for each terrain type (pine trees, sheep, wheat stalks, brick stacks, mountain peaks, sand dunes) — no emojis
- **Resource Stats Dashboard** — Pip distribution bar chart per resource with balance score rating

### Visual Design
- **Custom SVG Terrain Illustrations** — All hex tiles across every page use hand-drawn SVG icons instead of emojis for a game-like feel
- **Rich SVG Diagrams** — Hex board, game pieces, resource cards, robber scenes, dev card fan, harbor trades, VP breakdowns — all pure SVG
- **Interactive Dice Roller** — Roll animation with shake effect, running roll counter, and a 7 triggers the robber indicator
- **Probability Chart** — Visual bar chart showing dice roll distributions (why 6 and 8 are the best tiles)
- **Victory Point Tracker** — Click circles to track your VP from 1–10 with celebration message

### Technical
- **Mobile-First Responsive** — Works perfectly on phones, tablets, and desktops
- **Zero Dependencies** — Pure HTML/CSS/JS, no frameworks, no build step
- **Dark Mode Support** — Automatic dark mode based on system preference
- **Sticky Navigation** — Tabbed interface with smooth scroll, always accessible

## 📸 What's Inside

### Landing Page (`/`)
- Guide cards with real board game photos for Base Game and Seafarers
- Scrolling "Coming Soon" ticker announcing upcoming expansion guides
- Map Randomizer tool card

### Base Game Guide (`/base`)
| Section | Visual Highlights |
|---------|------------------|
| **Overview** | 5 resource cards with SVG terrain icons, core game loop |
| **Setup** | 6 component cards, board assembly diagram, distance rule visual |
| **Your Turn** | Dice → hex → resource flow, player trade & bank trade diagrams |
| **Building** | Game piece showcase with cost grid |
| **Trading** | 3 harbor rate cards (4:1, 3:1, 2:1) |
| **Robber** | Robbery scene with blocked hex, steal card illustration |
| **Dev Cards** | Fanned card spread showing all 5 types with counts |
| **Winning** | VP sources illustrated, interactive tracker |
| **Almanac** | Searchable A–Z rules reference (40+ entries) |
| **Dice Tool** | Animated roller + probability bar chart |

### Seafarers Guide (`/seafarers`)
| Section | Visual Highlights |
|---------|------------------|
| **Overview** | What's new, what stays the same, terrain hex legend with SVG icons |
| **What's New** | Board changes, trade routes, settling new islands |
| **Ships** | Building, moving, open vs closed routes |
| **Special Tiles** | Gold hexes, fog tiles, pirate mechanics |
| **Building Costs** | Ship + all base costs |
| **Scenarios** | All 9 official scenarios with VP targets |
| **Strategy** | 6 expansion-specific tips |

### Map Randomizer (`/randomizer`)
| Feature | Details |
|---------|---------|
| **Board Rendering** | Ocean frame, gradient terrain hexes, sandy coastline, water hex ring |
| **Number Tokens** | Cream radial gradient with drop shadows, red 6/8 highlighting, pip dots |
| **Terrain Icons** | SVG pine trees, sheep, wheat, bricks, mountains, sand dunes |
| **Controls** | 3–4 / 5–6 player toggle, balance rule checkboxes |
| **Stats** | Resource pip distribution bars + balance score |

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
│   ├── index.html          # Landing page — guide cards + coming soon ticker
│   ├── base.html           # Base game guide (9 tabs + almanac + dice tool)
│   ├── seafarers.html      # Seafarers expansion guide
│   ├── randomizer.html     # Map randomizer tool (balanced board generator)
│   ├── img-base-box.jpeg   # Base game card image
│   ├── img-seafarers-box.jpg # Seafarers card image
│   ├── logo.png            # Site logo
│   ├── og-image.png        # Open Graph social sharing image (1200×630)
│   ├── sitemap.xml         # XML sitemap for Google Search Console
│   ├── robots.txt          # Crawler directives + sitemap reference
│   └── favicon.*           # Favicons (SVG, PNG, ICO)
├── vercel.json              # Vercel config (caching, headers, security)
├── package.json             # Project metadata & scripts
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

All game rules are based on the **Catan 5th Edition** official rulebook and the **Seafarers** expansion rulebook by Klaus Teuber, cross-referenced with multiple established board game rules sources including catan.com, UltraBoardGames, BoardGameArena, and colonist.io.

> **Disclaimer:** This is an unofficial fan-made guide. CATAN is a registered trademark of Catan GmbH. This project is not affiliated with or endorsed by Catan GmbH or Catan Studio.

## 🛠️ Customization

Each page is a standalone HTML file — easy to modify:

- **Colors** — Edit the CSS variables in `:root` at the top of each HTML file
- **Content** — Sections are labeled with HTML comments (`<!-- ═══ SETUP ═══ -->`)
- **Add sections** — Add a new `nav-btn` + matching `section` element; the JS handles the rest
- **SVG illustrations** — All inline, editable directly in the HTML
- **Terrain icons** — Defined in `terrainIconSVG()` function (randomizer) and auto-injected via script (base game)

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
