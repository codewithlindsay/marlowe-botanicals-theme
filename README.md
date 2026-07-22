# Marlowe Botanicals — Shopify theme

A custom Shopify theme (Online Store 2.0, built on **Dawn**) for Marlowe Botanicals —
small-batch botanical oils & massage therapy. Reproduces the Lonnie/Marlowe design
references section-for-section.

- **Palette:** lavender `#E8D8F8` · plum `#5B4373` · mint `#E4EFD1` · lime `#A9CC7B` · cream `#FDF3EA` · charcoal `#3F3F3D`
- **Fonts:** DM Serif Display (display) + Space Mono (body), loaded via Google Fonts in `layout/theme.liquid`

## Custom sections

Each labeled section in the design maps to one file in `sections/`:

| Handle | Type | Used on |
| --- | --- | --- |
| `announcement-bar` | announcement bar | all (header group) |
| `header` | header | all (header group) |
| `footer` | footer | all (footer group) |
| `hero-banner` | image banner | home |
| `featured-bestsellers` | featured collection (card blocks) | home |
| `slow-down` | image with text + checklist | home |
| `marquee` | scrolling text | home |
| `seasonal-candles` | featured collection (card blocks) | home |
| `faq` | collapsible content | home |
| `services` | multicolumn | home |
| `testimonials` | testimonials | home |
| `about-founder` | image with text | home |
| `newsletter` | newsletter (customer form) | home |
| `breadcrumb` | breadcrumb | product |
| `product-info` | main product (variants, add-to-cart, accordions) | product |
| `related-products` | related products | product |
| `page-hero` | rich text banner | about, contact |
| `story` | image with text | about |
| `values` | multicolumn | about |
| `founder-quote` | rich text | about |
| `cta` | rich text | about |
| `booking-form` | contact form | contact |

Templates: `templates/index.json` (home), `templates/product.json`,
`templates/page.about.json`, `templates/page.contact.json`.

## Connect to a Shopify dev store (GitHub integration)

1. In your Shopify admin: **Online Store → Themes → Add theme → Connect from GitHub**.
2. Authorize GitHub if prompted, choose this repo (`marlowe-botanicals-theme`) and the `main` branch.
3. Shopify adds the theme to your library. Click **Customize** to edit in the theme editor;
   commits pushed to `main` sync automatically.

### Set up pages & menus (one-time, in admin)

- **Pages → Add page** for *About* (template `page.about`) and *Contact* (template `page.contact`).
- **Navigation → Main menu**: add Shop / About / Journal links; the header's "Book a session"
  button and its links are set in the theme editor (Header section).
- Everything renders with the design's placeholder copy out of the box; swap images and text
  in the theme editor.

## Local development (optional)

With the [Shopify CLI](https://shopify.dev/docs/themes/tools/cli):

```bash
shopify theme dev --store your-store.myshopify.com
```
