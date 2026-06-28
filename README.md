# TrendIT Systems — Website

Official website for **TrendIT Systems**, a business based in Kubwa, Abuja, Nigeria offering Solar & Inverter installation, IPTV subscriptions, and Technology/IT support services.

**Live site:** https://trendit-solar.vercel.app

---

## 📁 Project Structure

```
trendit-solar/
├── index.html          # Main website (single-file: HTML + CSS + JS)
├── sitemap.xml          # Search engine sitemap
├── robots.txt           # Search engine crawl rules
└── images/
    ├── logo.jpg          # Brand logo (original, grey background)
    └── logo-nobg.png     # Brand logo (transparent background)
```

---

## 🧩 Tech Stack

- **HTML5** — semantic markup
- **CSS3** — no frameworks, custom properties (CSS variables) for theming
- **Vanilla JavaScript** — no libraries, used for:
  - Sticky navbar on scroll
  - Mobile hamburger menu
  - Scroll-reveal animations (Intersection Observer)
- **Hosting** — [Vercel](https://vercel.com)
- **Fonts** — Google Fonts (`Fraunces` for headings, `DM Sans` for body)

No build step, no dependencies, no `node_modules`. Just static files.

---

## 🎨 Brand Colors

| Variable | Hex | Used for |
|---|---|---|
| `--green-deep` | `#1a4731` | Hero background, dark sections |
| `--green-mid` | `#246b47` | Primary buttons, accents |
| `--green-light` | `#34a05a` | Highlights, hover states |
| `--gold` | `#f0b429` | Accent color (solar/energy theme) |
| `--blue-mid` | `#1f6fa8` | Secondary accent (tech/IT touch) |
| `--blue-deep` | `#16314f` | Secondary accent (dark variant) |
| `--charcoal` | `#1c2630` | Footer background, dark text |
| `--cream` | `#fafaf7` | Page background |

To adjust brand colors, edit the `:root` block at the top of the `<style>` section in `index.html`.

---

## 📄 Sections (in order)

1. **Navbar** — sticky, with Services dropdown (Solar/IPTV/IT submenu) + mobile hamburger menu
2. **Hero** — headline, service pills, WhatsApp CTA, live stats
3. **Services** — 3 service cards: Solar & Inverter (flagship), IPTV, Technology & IT Support
4. **Pricing** — Solar/Inverter packages grouped by voltage category (12v / 24v / 48v)
5. **Why Choose Us** — 4 trust-building points
6. **Projects** — sample completed installations
7. **Testimonials** — customer reviews
8. **Call to Action** — final WhatsApp push
9. **Footer** — contact info, address, social links, sitemap links

---

## 📞 Contact Info on Site

| Type | Value |
|---|---|
| Address | Shop 8, Kubwa Central Market, Kubwa, Abuja, 901101 |
| Phone (primary/WhatsApp) | 0703 545 8331 |
| Phone (secondary) | 0806 894 3310 |
| Email | support@trenditsystems.com.ng |
| Facebook | [web.facebook.com/TrendITSystems](https://web.facebook.com/TrendITSystems) |
| Instagram | [@trendit_systems](https://www.instagram.com/trendit_systems/) |

> ⚠️ If any of these change, search the file for the old value and replace **all instances** — phone numbers and the WhatsApp link (`wa.me/2347035458331`) appear multiple times throughout `index.html` (nav, hero, services, pricing, footer, floating button).

---

## 🔍 SEO Setup

Already implemented:
- ✅ Meta title, description, keywords
- ✅ Open Graph + Twitter Card tags (for link previews on WhatsApp/Facebook/Instagram)
- ✅ Canonical URL tag
- ✅ `LocalBusiness` structured data (JSON-LD) — includes address, phone, services offered
- ✅ `sitemap.xml` and `robots.txt`

**Still to do manually (not code-based):**
- [ ] Submit sitemap to [Google Search Console](https://search.google.com/search-console)
- [ ] Set up & verify [Google Business Profile](https://business.google.com)
- [ ] Set up WhatsApp Business profile + catalogue

---

## 🚀 Deployment

Hosted on **Vercel**. To redeploy after making changes:

```bash
cd trendit-solar
vercel --prod
```

If not yet linked to a Vercel project:

```bash
vercel
```

and follow the prompts (project name: `trendit-solar`, root directory: `.`).

---

## 🛠️ Common Edits

| To change... | Edit this... |
|---|---|
| WhatsApp number | Find/replace `2347035458331` (international format, no `+` or spaces) |
| Pricing packages | `#pricing` section — each `.package-card` has specs + price |
| Service descriptions | `#services` section — each `.service-card` |
| Testimonials | `#testimonials` section — each `.testimonial-card` |
| Logo | Replace `images/logo.jpg`, keep the same filename or update all `<img src="images/logo.jpg">` references |
| Colors | `:root` CSS variables at the top of `<style>` |

---

## 📋 Pending / Next Steps

- [ ] Add real project photos (currently using styled placeholder graphics in the Projects section)
- [ ] Wire up Formspree contact form (endpoint pending from client)
- [ ] Connect custom domain (currently on `.vercel.app` subdomain)
- [ ] Google Business Profile setup
- [ ] Begin content/social posting schedule
- [ ] First paid ad test (Facebook/Instagram)

---

## 👤 Maintained By

Built by **Joseph Okoemu (Wayne)** — Axion Digital
- GitHub: [Waynemandem](https://github.com/Waynemandem)
- Twitter/X: [@Joseph_mandem](https://twitter.com/Joseph_mandem)

---

*Last updated: June 2026*
