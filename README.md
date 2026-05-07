# Reshma Beauty — Henna Haircare Newsletter

Production-ready responsive HTML email promoting the Henna Shampoo + Conditioner with a 30% bundle discount.

## File structure

```
.
├── index.html               Email template (table-based, inline CSS)
└── images/                  Compressed assets (~580 KB total)
    ├── logo-reshma.png
    ├── hero-banner.jpg
    ├── shampoo-bottle.jpg
    ├── conditioner-bottle.jpg
    └── botanical-lifestyle.jpg
```

## Tech specs

- 600 px container with mobile-first media query at `max-width: 600px`
- Table-based layout, inline CSS, no JS, no web fonts
- Tested-friendly with: Gmail, Outlook (mso conditionals), Apple Mail, Mailchimp
- Total weight: HTML ~32 KB + images ~580 KB = under 1 MB ✓

## Color palette

| Role | Hex |
|---|---|
| Background | `#F9F9F7` |
| Primary green | `#1B3B26` |
| Secondary green | `#3D6346` |
| CTA brown | `#704F37` |
| Accent gold | `#F2C94C` |
| Text | `#1A1A1A` |

## Deployment

1. Open `index.html` in a browser to preview locally.
2. Upload to your ESP:
   - **Mailchimp**: Templates → Create → Code your own → Paste in code → upload images via the campaign builder
   - **Klaviyo**: Templates → Create New → HTML editor → paste source → host images on Klaviyo CDN
3. Replace relative `images/...` paths with absolute CDN URLs once images are uploaded.

## UTM tracking

All 5 CTAs carry the same campaign tag:

```
?utm_source=email&utm_medium=newsletter&utm_campaign=henna_bundle_30
```

`utm_content` differs per placement: `hero_cta`, `product_shampoo`, `product_conditioner`, `bundle_primary`, `bundle_reinforce`.

## Pre-send checklist

See the open to-do list (in chat / project notes) for the remaining items: legal address, ESP merge tags, real social icons, Shopify discount code, Litmus QA.
