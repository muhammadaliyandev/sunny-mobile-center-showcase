# Sunny Mobile Center — POS (Showcase)

> **Showcase only — this repo contains no source code.**
> It shows a live point-of-sale system that is in daily use at a mobile shop in Bahawalnagar, Pakistan. The live shop system itself stays private.

**Live demo:** https://sunny-mobile-center.pages.dev

![Dashboard](screenshots/dashboard.png)
![Billing](screenshots/billing.png)
![IMEI check](screenshots/imei-check.png)

## What it does

- **Billing** — tappable product grid with search and category filters, cart with quantity steppers, per-item and total-bill discounts, Cash or Udhaar payment, automatic bill numbers, and bills that can be shared on WhatsApp or printed / saved as PDF.
- **Barcode scan** — scan with the phone camera and the product fills itself into the bill.
- **Udhaar ledger** — every customer with what they owe, a detail page with all credit bills and payments, partial or full payments, and balances that update automatically.
- **IMEI system** — Luhn validation, stock / sold tracking, bills linked to IMEIs, and any-phone identification from self-hosted open data (275,848 TACs + 8,556 specs). Scan-to-auto-fill, hand-typed IMEIs, unknown models flagged for manual entry, and deleting a product cascades its IMEIs.
- **Dashboard & reports** — today's sales and profit, bills today, low-stock items, total udhaar to collect, plus period reports (Today / 1 Week / 4 Weeks / This Month / custom range) with a daily sales chart, printable PDF report and CSV export.
- **Mobile-first PWA** — installable on an Android home screen, works offline with bill sync.

## Tech stack

- Frontend: React + Vite, React Router, vite-plugin-pwa (Workbox)
- Backend: Node.js + Express, JWT auth, bcrypt
- Database: MongoDB with Mongoose (MongoDB Atlas)
- Hosting: Cloudflare Pages (frontend) + Oracle Cloud VM with Caddy and Docker (backend)

## Why it matters

This is not a tutorial project — it is a real shop system handling real bills, stock and credit every day, built because the shop competes with bigger stores on phone prices and needs profit from accessories, services and clean record-keeping.

---

*Screenshots: replace the three placeholder images in `screenshots/` with real phone screenshots of the dashboard, billing screen and IMEI check. Do not include any bill or customer screen that shows a real customer's name, phone number or IMEI.*
