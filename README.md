# SPENDTrack

> Personal expense tracker — offline-first PWA, no account needed.

---

## Overview

SPENDTrack lets you log, categorize, and visualize personal spending entirely on-device. No server. No sign-up. All data stays in your browser.

---

## Features

- **Expense logging** — Add expenses with amount, category, date, and optional note
- **Multiple accounts** — Separate tracking across Cash, Savings, and custom account types
- **Categories** — User-defined spending categories with full CRUD
- **Charts** — Pie and bar chart breakdowns by category and time period
- **Import / Export** — Full data portability via CSV
- **Native Share** — Share expense summaries via Web Share API
- **Offline-first** — Cache-first service worker; works with no connection after first load
- **Installable** — Add to home screen on Android and iOS

---

## Tech

| Layer | Detail |
|---|---|
| Stack | Single-file HTML · Vanilla CSS · Vanilla JS |
| Storage | `localStorage` |
| Charts | `<canvas>` + Chart.js |
| Offline | Service Worker (cache-first for assets, network-first for fetches) |
| Install | Web App Manifest · PWA |
| Share | `navigator.share` |

---

## Getting Started

No build step. No dependencies to install.

```bash
git clone https://github.com/yourusername/SPENDTrack-PWA.git
cd SPENDTrack-PWA
# Open index.html in a browser, or serve locally:
npx serve .
```

For PWA install prompt and service worker to activate, serve over **HTTPS** or `localhost`.

---

## File Structure

```
SPENDTrack-PWA/
├── index.html       # Entire app
├── manifest.json    # PWA manifest
├── sw.js            # Service worker
└── icons/           # PWA icons (72px – 512px)
```
