# Beltim × Joby RFQ Dashboard

Static single-page dashboard tracking the Joby JCD02 Pit Dispenser (GSE) RFQ across HiTech, JF Precision, ALW, PNM, POP, and Carlos weld vendors.

Auto-deployed to Vercel on every push to `main`. Updated twice daily by a scheduled job that searches Gmail for vendor replies and patches `COMPARE_DATA` in `index.html`.

## Files

- `index.html` — the full dashboard (6 pages, self-contained)
- `vercel.json` — Vercel static-site config (no-cache on index so updates are immediate)
- `.last-check.json` — timestamp of the most recent scheduled run (used to search Gmail for only new replies)
