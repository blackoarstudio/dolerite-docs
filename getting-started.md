---
title: "Getting started"
description: "Install Dolerite, work through the setup checklist, and publish. Also: how to move to a newer version of the theme."
---
# Getting started

## 1. Install the theme

1. In your Shopify admin, go to **Online Store → Themes**.
2. Under *Theme library*, choose **Add theme → Upload zip file** and select the
   Dolerite zip.
3. Click **Customize** to open the theme editor. The theme is not live yet — visitors
   still see your current theme until you publish.

Work through the rest of this page before you publish. Everything below is reversible.

## 2. What ships on the home page

The home page arrives with four sections in this order:

1. **Hero** — headline, subheading and one button.
2. **Product grid** — four products.
3. **Editorial split** — two images beside a block of text.
4. **Product grid** — two products, set up as a smaller "capsule" row.

The text in these sections is placeholder copy that describes what belongs there.
Replace it. The product grids have no collection selected yet, so they render grey
placeholder cards until you pick one — that is the theme telling you the setting is
empty, not an error.

## 3. The setup checklist

Do these seven things and the store is ready to look at.

### Logo and favicon

Theme editor → **Theme settings → Branding**.

- **Logo** — shown in the header. A transparent PNG works best.
- **Logo text** — shown next to the logo. Leave it empty and your store name is used.
- **Logo height** — 28 to 72 px.
- **Favicon** — the icon in the browser tab. Use a square image; browsers draw it at
  32 × 32 px.

### Menus

Dolerite reads two menus, and both are pre-selected:

| Menu handle | Where it appears | Setting |
| --- | --- | --- |
| `main-menu` | Header and mobile drawer | Header section → **Navigation menu** |
| `footer` | Footer | Footer section → **Footer menu** |

Both menus already exist in every Shopify store. Edit them under **Content →
Menus**. If you build a menu under a different handle, point the section setting at
it instead.

A top-level item with **three levels** of menu items below it opens as a mega menu.
See [Navigation and search](navigation.md).

### Colors

Theme editor → **Theme settings → Colors**.

Four color schemes ship with the theme. **Page color scheme** decides which one paints
the store itself — header, footer, cart and every section left on the default. Change
that one setting and the whole store follows.

Every section also has its own **Color scheme** setting, so you can put one section on
a different scheme to make it stand out as a band of color. Read
[Theme settings → Colors](theme-settings.md#colors) before you edit the schemes
themselves; the theme derives hairlines, muted text and accent tints from the colors
you set, so a small number of edits go a long way.

### Fonts

Theme editor → **Theme settings → Typography**. Three fonts, each picked from
Shopify's font library:

- **Display font** — headings.
- **Body font** — paragraphs, descriptions, form fields.
- **Detail font** — the small type set in capitals: eyebrows, buttons, prices, table
  labels. A monospace face keeps columns of figures lined up.

### Products in the grids

Open each **Product grid** section on the home page and choose a **Collection**. Set
**Products to show** and **Columns (desktop)** to taste.

### Pages every store needs

Create these under **Content → Pages**, then link them from the footer menu:

- A contact page. Create the page, and in **Theme template** choose `page.contact` —
  that template renders a working contact form.
- Your policies. Shopify generates refund, privacy, terms and shipping policies under
  **Settings → Policies**; they get their own URLs and belong in the footer menu.

### Cart style

Theme editor → **Theme settings → Cart**. **Let customers add a note to their order**
is on by default and shows a note field in both the cart drawer and the cart page.

## 4. Replace the placeholder text

Every default heading and paragraph in the theme is written to tell you what belongs
in that spot. None of it describes a real product, and none of it should survive to
your live store. Work through the home page section by section.

The testimonial section is the one to watch: its quotes are placeholders. Replace them
with real customer feedback or remove the section. Never publish an invented review.

## 5. Preview and publish

1. In the theme editor, use the device icons to check phone and tablet widths.
2. Close the editor and choose **Actions → Preview** to click through the real store:
   home → collection → product → cart.
3. When you are happy, **Actions → Publish**.

## Updating to a newer version of Dolerite

Theme updates arrive as a new zip. Shopify does not merge settings across uploads, so:

1. Upload the new zip as a second, unpublished theme.
2. Set it up alongside the live one — the editor lets you work on an unpublished theme
   without visitors seeing it.
3. Publish when it matches.

Keep the old theme in your library for a week or two before deleting it. If you edited
theme code, note those edits before you start; they do not carry over.
