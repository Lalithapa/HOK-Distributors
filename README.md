# 🧴 HOK DISTRIBUTORS – Shopify (Tailwind) E-commerce

![Shopify](https://img.shields.io/badge/Built%20With-Shopify-7AB55C?logo=shopify&style=flat-square)
![Tailwind](https://img.shields.io/badge/Styling-TailwindCSS-38B2AC?logo=tailwindcss&style=flat-square)
![Responsive](https://img.shields.io/badge/Responsive-Yes-2563EB?style=flat-square)
![License](https://img.shields.io/badge/License-Proprietary-AA0000?style=flat-square)

**HOK Distributors** is a wholesale/distributor version of HOK Makeup — optimized for **trade buyers** with gated access, tiered pricing, bulk ordering, and GST-compliant invoicing.  
Built with **Shopify + Tailwind CSS**, focused on speed, clarity, and operational efficiency.

🌐 **Live Website:** https://www.hokdistributors.com

---

## 🎯 What’s Different vs HOK Makeup (B2C)

- 🔒 **Gated Catalog** — collections & prices visible only after login
- 💰 **Trade Pricing** — tiered price lists, MOQs, volume breaks
- 🧾 **GST/Tax-Ready** — GST fields at onboarding & tax invoice support
- 🛒 **Bulk Ordering** — quantity steppers, quick-add grids, CSV upload
- 🧮 **Net Terms & PO** — optional purchase order field on cart/checkout
- 💬 **WhatsApp Sales Desk** — pre-filled SKU inquiries, order assistance
- 🚚 **Distributor Shipping Rules** — carton/weight-based & prepaid slabs

---

## 🎨 Features

- ✅ Custom Shopify theme with **TailwindCSS** utility classes
- ✅ Fully responsive layout (mobile-first)
- ✅ **Variant swatches** & trade badges (e.g., “MOQ 6”, “Case of 24”)
- ✅ **Login wall** + redirect rules (unauthenticated → `/account`)
- ✅ **Metafield-driven** banners (desktop/mobile via `<picture>`)
- ✅ **Quick Order** section (grid & list modes)
- ✅ **Bulk Add to Cart** with debounced updates
- ✅ **Account area** with wholesale docs, credit limits (content)
- ✅ Core Web Vitals optimization (LCP/CLS/INP) 🚀

---

## 🛠️ Tech Stack

| Tech           | Purpose                                  |
|----------------|-------------------------------------------|
| **Shopify**    | Storefront + backend                      |
| **Liquid**     | Theme templating                          |
| **TailwindCSS**| Utility-first styling                     |
| **Alpine/JS**  | Lightweight interactivity (no jQuery)     |
| **Metafields** | Content & pricing flags                   |
| **Shopify CLI**| Local dev, preview, deploy                |

---

## ⚙️ Getting Started

### 1) Install & Link
```bash
# Install deps
npm i

# Tailwind build (dev)
npm run dev

# Shopify build (dev)
npm run theme

# Shopify preview (login once via CLI)
shopify theme dev

// package.json (excerpt)
{
  "scripts": {
    "dev": "tailwindcss -i ./src/input.css -o ./assets/theme.css --watch",
    "build": "NODE_ENV=production tailwindcss -i ./src/input.css -o ./assets/theme.css --minify"
    "theme": "theme watch --allow-live"
  }
}
