---
title: "Theme settings"
description: "Every store-wide setting in Dolerite: branding, color schemes, typography, background, layout, social links, cart, product cards and motion."
---
# Theme settings

These are the store-wide settings. Open the theme editor and click the gear icon at
the bottom of the left sidebar, or choose **Theme settings** from the section list.
Nine groups, in the order they appear.

Dolerite installs in one of three styles: **Dolerite**, **Alabaster** or
**Anthracite**. A style is a set of starting values for the settings on this page,
nothing more — every one of them can be changed. Where the three start from different
values, this page says so. These start differently and are not repeated below:

| Setting | Dolerite | Alabaster | Anthracite |
| --- | --- | --- | --- |
| **Colors** | Near-black, teal accent | Warm off-white, rust accent | Blue-black, light blue accent |
| **Display font** | Instrument Serif | Playfair Display | Archivo |
| **Body font** | Inter | DM Sans | Inter |
| **Detail font** | IBM Plex Mono | Space Mono | IBM Plex Mono |
| **Products per row on phones** | One | Two | Two |
| Product cards → **Image shape** | Square | Portrait | Square |
| Product cards → **Text alignment** | Left | Center | Left |

- [Branding](#branding)
- [Colors](#colors)
- [Typography](#typography)
- [Background](#background)
- [Layout](#layout)
- [Social media](#social-media)
- [Cart](#cart)
- [Product cards](#product-cards)
- [Motion](#motion)

---

## Branding

| Setting | What it does |
| --- | --- |
| **Logo** | Shown in the header next to the logo text. A transparent PNG works best. |
| **Logo text** | Shown next to the logo. Falls back to your store name when empty. |
| **Logo height** | 28–72 px, in steps of 4. Starts at 44 (Dolerite), 40 (Alabaster) or 36 (Anthracite). |
| **Favicon** | The icon in the browser tab. Use a square image — browsers draw it at 32 × 32 px. |

The logo text is always shown — your own, or the store name when the field is empty.
Add a logo image and it sits left of the text.

---

## Colors

This is the setting group that carries the most weight in Dolerite, so it is worth
five minutes.

### How color works in this theme

A **color scheme** is a named set of six colors. The theme ships with four. Every
section you add, and the footer, has a **Color scheme** setting, so you decide per
section which of them it uses — that is how you get alternating bands of color down a
page without ever typing a color value twice.

**Page color scheme** picks the scheme for the page itself: the header, the cart
drawer and the sections behind each page type — product, collection, cart, search, the
customer account pages — which have no color setting of their own.

A section's **Color scheme** starts on Scheme 1, and so does **Page color scheme**. A
section on the page's scheme blends into the page; a section on any other scheme is
drawn as a band in that scheme's colors. So if you move **Page color scheme** to
another scheme, the sections still set to Scheme 1 — the footer among them — stay on
Scheme 1 and become bands. Switch them as well if the whole store should follow.

### The six colors in a scheme

| Color | Used for |
| --- | --- |
| **Background** | The page behind everything. |
| **Surface** | Cards, drawers and form fields — the panels that sit on the background. |
| **Text** | Body text and headings. |
| **Muted text** | Descriptions and secondary lines. |
| **Accent** | Buttons, links, focus rings, highlights. |
| **Text on accent** | The label printed on an accent-filled button. |

Some of these do more than they look like they do. **Text** and **Background** are
mixed to produce the hairlines. **Muted text** and **Background** are mixed to produce
the dimmest labels. The tints behind badges and highlights are **Accent** at low
strength. Set those four well and the rest of the scheme falls into place. It also
means a light scheme never ends up with black hairlines drawn on white paper — the
theme recomputes them from the scheme's own colors.

**Text on accent** is the one people forget. On a dark scheme with a bright accent it
needs to be dark. On a light scheme with a deep accent it needs to be light. If your
button labels are hard to read, this is the setting.

### The four schemes that ship

| Scheme | Character |
| --- | --- |
| Scheme 1 | The page itself. Dark with a bright accent in the Dolerite and Anthracite styles, light with a deep accent in Alabaster. The default. |
| Scheme 2 | One step away from scheme 1 — for a section that should lift off the page. |
| Scheme 3 | A background in the accent's hue. A full-bleed color band. Use sparingly. |
| Scheme 4 | The opposite of scheme 1: light in the two dark styles, dark in Alabaster. |

Edit any of them, or press **Add scheme** for a fifth. Schemes are numbered in the
order they are created, and a section keeps pointing at the scheme it was assigned.

### Checking contrast

Shopify's Theme Store requires an accessible storefront and so do your customers. If
you change the colors, check that:

- **Text** on **Background** and on **Surface** is easy to read.
- **Text on accent** is easy to read on **Accent**.
- **Muted text** is still legible — it is deliberately quieter than **Text**, so it is
  the first thing that breaks when a scheme is edited.

A free contrast checker such as WebAIM's takes a foreground and a background hex value
and gives you a ratio. Aim for 4.5:1 or better on running text.

---

## Typography

| Setting | Used for |
| --- | --- |
| **Display font** | Headings and large statements. The weight you pick is the weight your headings get. |
| **Body font** | Paragraphs, product descriptions, form fields. |
| **Detail font** | The small type set in capitals: eyebrows, buttons, prices, table labels. |
| **Body text size** | 14–18 px. Starts at 15 (Dolerite), 16 (Alabaster) or 14 (Anthracite). |

All three come from Shopify's font library, which is served from Shopify's own CDN.
No external font service is contacted when a page loads.

Two things worth knowing:

- **A monospace Detail font keeps figures aligned.** Prices in a grid, quantities in a
  table and order numbers all line up in columns. The theme sets the weights for these
  elements itself, so only the family you pick has an effect.
- **Body text size moves running text only** — descriptions, answers, intros and form
  fields. Headings, prices and card labels keep the scale the theme sets for them, so
  raising it will not knock your layout out of proportion.

---

## Background

An optional pattern tiled behind the whole store, fixed while the page scrolls.

| Setting | Range |
| --- | --- |
| **Background pattern** | Any image. Subtle, dark, seamlessly tiling patterns work best. |
| **Pattern opacity** | 2–40 %. Starts at 25 (Dolerite), 6 (Alabaster) or 10 (Anthracite). |
| **Pattern tile size** | 400–1400 px. Starts at 900 (Dolerite), 1100 (Alabaster) or 700 (Anthracite). |

Leave the image empty for a flat background. The pattern sits behind sections that use
the page color scheme; a section set to a *different* scheme paints its own background
and covers the pattern for its height. That is intentional — it is how a color band
reads as a band.

---

## Layout

| Setting | What it does |
| --- | --- |
| **Max content width** | 960–1600 px. Starts at 1200 (Dolerite), 1400 (Alabaster) or 1300 (Anthracite). How wide content is allowed to grow on a large screen. |
| **Products per row on phones** | One or two. Applies to every product, collection and article grid in the store. Tablets always show two. |

---

## Social media

Paste the full address of each profile you want linked in the footer. Leave a field
empty and its icon is not shown.

Instagram · Facebook · TikTok · YouTube · Pinterest · X · Threads · LinkedIn

Use the full URL, including `https://`.

---

## Cart

| Setting | What it does |
| --- | --- |
| **Let customers add a note to their order** | On in the Dolerite and Alabaster styles, off in Anthracite. Shows a note field in the cart drawer and on the cart page. The note appears with the order in your admin. |

---

## Product cards

These settings apply to every product tile in the store — home page grids, collection
pages, search results, related products, everywhere.

| Setting | Options |
| --- | --- |
| **Image shape** | Square · Portrait · Tall portrait · Landscape. Photos are cropped to fill the shape unless a section is set to show the full image. |
| **Text alignment** | Left or Center. |
| **Show the second photo on hover** | On by default. Products with one photo are unaffected. Ignored on touch devices, which have no hover. |
| **Mark sold-out products** | On by default. |
| **Show the discount as a percentage** | Off in the Dolerite and Alabaster styles, on in Anthracite. Shows "−30%" instead of "Sale". |

Any other badge comes from a product tag. A product tagged `badge:Bestseller` shows a
**Bestseller** badge — see [Tags and metafields](tags-and-metafields.md#product-badges).

**Image shape is the setting to get right first.** Pick the one that matches how your
photography is framed, and shoot to it from then on. Mixed aspect ratios in one grid
are the most common reason a store looks untidy, and no setting can fix that
afterwards.

---

## Motion

| Setting | What it does |
| --- | --- |
| **Custom cursor** | Replaces the mouse pointer with a branded dot and trailing ring on desktop. Automatically off on touch devices and for visitors who prefer reduced motion. |
| **Button spotlight** | A soft highlight follows the mouse pointer across buttons. Desktop only: touch devices have no pointer to follow. The highlight is a lighter shade of your accent color, and the theme only shows it where the button label stays readable on it — with some color combinations you will see no highlight at all. |
| **Page transitions** | One page fades into the next, and a product photo travels from its card into the product page. Browsers that do not support this change pages as usual. |
| **Back to top button** | Appears in the bottom corner once the visitor has scrolled past one screen. |

All four start switched on, except **Custom cursor** in the Alabaster style. Every animation in the theme — the cursor, the hero entrance,
the scroll reveals, the slideshow — stops for visitors whose device is set to reduce
motion. You do not need to configure that; the operating system tells the browser and
the theme listens. The button spotlight is the exception, because it is not an
animation: it moves only when the visitor moves the pointer.
