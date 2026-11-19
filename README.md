# Growth Audit — F.A.Z. Kiosk

**Live:** https://bterzic123.github.io/faz-flow-rebuild/

Your readers get tomorrow’s paper at 18:00 the evening before. A new install never hears it. Today a new F.A.Z. Kiosk install accepts the consent screen, lands on the shelf under two iOS prompts at once, and meets „Wählen Sie Ihr Angebot für die digitale Ausgabe“ only after tapping a locked issue. This audit rebuilds that first launch in the Kiosk’s own design and at its own prices: it asks how the reader reads (E-Paper or Edition) and which section comes first, then shows an offer that names both.

The page has two views: an **Overview** with the five ideas, and a **Prototype** with three phones (a paper reader, a finance reader, a culture reader) you can tap through, plus a 30-second walkthrough.

## The five ideas

| # | Idea | Screen | Expected effect |
| :-- | :-- | :-- | :-- |
| 1 | Offer the subscription once, at the end of first launch | Offer | CR +10–20% |
| 2 | Name their section and format in the headline | Offer | CR +15–20% |
| 3 | Select the Monatsabo for them and print what month four costs | Offer | CR +5–15%, ARPU +3–8% |
| 4 | Put your 4.5 stars and a reader’s words next to the price | Offer | CR +10–15% |
| 5 | Ask for notifications after the offer, as an 18:00 alert | Shelf | CR +10–15% |

Impact ranges are Adapty’s expected effect from teardowns and A/B tests across subscription apps, not measured lift for F.A.Z. Kiosk.

## Grounding

Screens, copy and prices (Monatsabo 25,99 € a month for 3 months, then 54,90 € a month; F.A.Z. Einzelausgabe 3,99 €) come from the F.A.Z. Kiosk iOS app as recorded on 19 November 2026 on the German storefront. The rating (4.5 from 13,076 ratings), “über 1.100 Preise und Auszeichnungen”, “bereits am Vortag ab 18 Uhr”, the section names and the quoted review come from the German App Store listing. The Meta ads and their dates are as seen by AppMagic. No trial, discount or statistic was invented.

## Run locally

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000/ (or http://localhost:8000/?view=proto for the prototype).

Prepared by Adapty · [Book a demo](https://calendly.com/d/cty4-37z-zqj)
