# Dive Tend — marketing site

Static site for **divetend.com**, built to the same shape as ClearNight's
`marketing-site/`: plain HTML, no build step, GitHub Pages via `CNAME`.

| File | Purpose |
|---|---|
| `index.html` | Landing page |
| `privacy.html` | Privacy Policy — **Apple requires this URL to resolve before submission** |
| `terms.html` | Terms of Use |
| `support.html` | Support page — the Support URL in App Store Connect |
| `styles.css` | Shared tokens and components for all four pages |
| `CNAME` | `divetend.com` |
| `app-ads.txt` | AdMob publisher record |

## Differences from ClearNight's site, and why

- **One shared `styles.css`** rather than per-page inline `<style>`. Four
  pages that must not drift is the case for a single file.
- **Dive Tend's own palette and Montserrat**, the typeface the app is set in.
  Same system, same company — siblings rather than the same app twice.

## Before this goes live

- [ ] Replace `[EFFECTIVE DATE]` in `privacy.html` and `terms.html` — both
      carry it once. It should be the publication date, not the drafting one.
- [ ] Confirm the **Supabase backup retention window** and state it in
      Privacy → *How long we keep it*. The placeholder is marked inline.
- [ ] Decide the **EU/UK Article 27 representative** — appoint and name them
      in Privacy → *Your rights*, or delete that line.
- [ ] Verify `app-ads.txt` against the real AdMob account. The publisher ID
      is copied from ClearNight on the assumption of one AdMob account for
      Strange Glyph. **If that is wrong, ad revenue is affected.**
- [ ] Add `favicon.png` and an `icon.png` once the app icon exists.
- [ ] Set `LEGAL_HOST` in the app so the four in-app legal links resolve
      here. Until then they truthfully say "not published yet".

## Not written

A cookie notice. The site sets no cookies and loads no analytics — only
Google Fonts. If analytics is ever added, that changes.
