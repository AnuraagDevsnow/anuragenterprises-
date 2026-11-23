# Anurag news v2

A fast, zero-AI-summary news finder that runs in a single `index.html` file and uses the visitor's own browser (`localStorage`) for caching, keyword matching, deduplication, and sorting.

## Features

- **Topic Chips & Custom Presets:** Toggle ready-made topics (`AI & Tech`, `Trends`, `Investing & Markets`, `Fun & Gaming`, `Startups`) and save/apply/delete custom search presets.
- **Fast Client-Side Keyword Engine:** Supports exact phrases (`"..."`), word stemming, title/snippet weighting, and instant re-filtering as you type.
- **Today, Historical Dates & Date Ranges:** Search recent headlines, enter a single date in `DD/MM/YYYY` format (such as `20/11/2020`), or open a `From` – `To` date range.
- **Sorting & Story Grouping:** Sort results by `Relevant`, `Hot`, or `Old`, load headlines in batches of 20 on scroll, and collapse near-duplicate coverage (`+N similar`).
- **Local PC Cache & Offline Fallback:** Caches search results locally in `localStorage` with cache-age tags, a `Refresh Live` option, and clean fallback sample headlines if live feeds are unreachable or rate-limited.
- **Domain Muting, Sharing & Export:** Mute noisy domains, copy individual links, copy a shareable query URL (`Share link`), reset filters, and export results as plain text or JSON.
- **Optional Custom API Keys:** Uses keyless `GDELT DOC 2.0` by default, with optional browser-stored keys for `NewsData.io` or `GNews.io` in **Settings**.

## Keyboard Shortcuts

- `/` — Focus the custom keyword input
- `R` — Reset active filters

## Running & Hosting

1. Open `index.html` directly in a browser or serve the folder with any static web server.
2. For full PWA/home-screen icon support when hosting on GitHub Pages or similar static hosts, place `favicon.ico`, `apple-touch-icon.png`, `android-chrome-192x192.png`, `android-chrome-512x512.png`, and `site.webmanifest` in the root directory alongside `index.html`.