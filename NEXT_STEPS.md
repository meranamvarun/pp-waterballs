# Monetization plan — what's done vs. what needs you

Based on `PP Waterballs — Copyright-Safe Monetization Plan` (2026-09-19).

## Done in this change

- **Content roadmap pages** (all original text/art, no Bhatti likeness, no verbatim
  sketch lines, no re-cut video, no reproduced articles):
  - `prospectus.html` — fake red herring prospectus (risk factors, use of funds, financials)
  - `gmp-tracker.html` — parody grey-market-premium ticker (nudges a fake number client-side)
  - `investor-relations.html` — fake shareholder letter + AGM minutes
  - `merch.html` — merch preview cards ("IPO Allottee", "5000% Subscribed" mug, sticker pack), marked "Coming Soon" until real designs/store exist
- **"In the Media" section** on the homepage rewritten as short original blurbs (2-3 sentences each) instead of a bare link list, still linking out to ET/Livemint rather than quoting them.
- **Affiliate CTA boxes** added to every page ("Open a Demat Account" etc.), currently pointing at the *plain, non-affiliate* broker sign-up pages (Zerodha/Groww/Upstox) so nothing is broken.
- **Buy Me a Coffee link** added to every footer, pointing at the confirmed account: `buymeacoffee.com/itsmekc`.
- Shared `style.css` extracted so new pages match the existing look.
- `sitemap.xml` updated with the new URLs.

## Still needs you (can't be done from code / needs your identity+bank details)

1. **Broker affiliate programs.** Sign up for the Zerodha / Groww / Upstox partner
   programs (needs your PAN/bank KYC). Once you have tracked referral links, replace
   the plain URLs in the `cta-box` sections — search for `TODO(owner)` in `index.html`
   and the affiliate `href`s in the other pages.
2. **Google AdSense.** Apply once this has run for a bit with real pages/traffic
   (approval needs a live site + your account). Once approved, drop the verification/
   ads snippet where `index.html` has an HTML comment marking the spot in `<head>`.
3. **Print-on-demand merch store.** Design the 2-3 t-shirt/mug/sticker graphics (text
   + your own artwork only — no Bhatti likeness, no verbatim sketch lines) and list
   them on Printrove/Qikink, then swap `merch.html`'s "Coming Soon" cards for real
   product links.
4. **Domain renewal.** Confirm it's cleared in Hostinger — outside this repo entirely.
5. **Newsletter/social account** riffing on "craziest IPO of the week" — a separate
   channel, not part of this static site.

## Explicitly skipped (per the plan)

- Anything implying Jaspal Bhatti or his estate endorsed the site.
- Reproducing his likeness/voice/verbatim lines anywhere, including merch.
- Re-cutting or re-uploading clips from the sketch.
- Using real IPO companies' logos/trademarks.
