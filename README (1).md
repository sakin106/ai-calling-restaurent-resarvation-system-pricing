# 📞 AI Phone Receptionist — Pricing Page

A clean, interactive pricing slide built in pure HTML/CSS/JS for an **AI-powered phone receptionist service** designed for restaurants. No frameworks, no build tools — just a single self-contained file ready to embed or share.

---

## ✨ Features

- **3-tier pricing cards** — Base, Growth (recommended), and Premium plans with clear feature breakdowns
- **Transparent cost breakdown** — Third-party infrastructure costs (Vapi, OpenAI, Cloud Server) displayed separately so clients always know what they're paying and to whom
- **Cost estimate summary** — Min / Typical / Max monthly infrastructure ranges at a glance
- **Interactive cost calculator** — Select a plan, drag sliders for call volume and average call duration, and see a live breakdown of total monthly cost including one-time setup fee
- **Print-friendly** — Clean `@media print` styles included for PDF/screenshot use

---

## 🗂️ Pricing Overview

| Plan    | Setup Fee | Monthly Fee | Call Limit         |
|---------|-----------|-------------|--------------------|
| Base    | $549      | $119/mo     | Up to 300 calls/mo |
| Growth  | $749      | $192/mo     | Up to 750 calls/mo |
| Premium | $1,119    | $249/mo     | Unlimited          |

> Infrastructure costs (Vapi, OpenAI, hosting) are **billed directly by third-party providers** and are separate from the service fee.

---

## 🏗️ Tech Stack

| Layer     | Choice                                                  |
|-----------|---------------------------------------------------------|
| Markup    | Semantic HTML5                                          |
| Styling   | Vanilla CSS (CSS Grid, Flexbox, CSS custom properties)  |
| Logic     | Vanilla JavaScript (no dependencies)                    |
| Fonts     | Google Fonts — DM Sans + DM Mono                        |

---

## 🚀 Usage

Just open `pricing-slide.html` directly in any browser — no server, no install required.

```bash
# Clone the repo
git clone https://github.com/your-username/ai-receptionist-pricing.git

# Open in browser
open pricing-slide.html
```

To embed inside an existing site, drop the file contents inside your layout or iframe it:

```html
<iframe src="pricing-slide.html" width="100%" height="900" frameborder="0"></iframe>
```

---

## 🧮 Calculator Logic

The monthly cost calculator estimates:

- **Service fee** — flat monthly rate from the selected plan
- **Vapi voice cost** — `calls × duration × rate` (rate range: $0.05–$0.12/min, midpoint used)
- **OpenAI processing** — tiered estimate based on call volume ($8 / $15 / $25)
- **Server hosting** — flat $10/mo

**Total = Service Fee + Vapi + OpenAI + Hosting**

---

## 📁 File Structure

```
/
└── pricing-slide.html   # Single self-contained file (HTML + CSS + JS)
```

---

## 🎨 Design Notes

- Color palette: warm off-white background (`#F5F4F0`), crisp white cards, dark featured plan (`#111`)
- Typography: DM Sans for UI text, DM Mono for prices and numbers
- Recommended plan highlighted with a green `Recommended` badge and inverted dark card style
- Cost summary uses color-coded tiers: green (min), amber (typical), red (max)

---

## 📄 License

MIT — free to use, modify, and distribute.
