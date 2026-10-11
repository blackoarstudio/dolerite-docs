---
title: "Troubleshooting"
description: "The settings and data behind the questions a theme support inbox actually receives."
---
# Troubleshooting

Most of what looks like a fault in a theme is a setting that is empty, a piece of data
that is missing, or something behaving exactly as designed in the theme editor but not
on the storefront. This page covers the cases we are asked about most.

If your question is not here, [get in touch](support.md).

## Content that is not appearing

### My product grid shows gray placeholder cards

The collection the section points at has no products, or no collection is selected.
Open the section and pick one under **Collection**. The placeholders are the theme
showing you the layout while there is nothing to show.

### My home page shows placeholder pictures, a "Product title" or a countdown

That is how a style installs, before your own content is in. A **Slideshow** or
**Editorial split** without images, a **Collection teaser** without collections, a
**Featured product** without a product and a **Drop** without a collection all draw
placeholders in the places your content will take. The countdown on the Anthracite home
page belongs to the **Drop** section's example launch time: set your own under **Launch
time**, clear it, or remove the section. See
[Getting started](getting-started.md#what-ships-on-the-home-page).

### Related products / Recently viewed show nothing

Both sections stay out of the way when they have nothing to show.

*Related products* asks Shopify for recommendations. A product it has none for yet
shows nothing — and so does one without complementary products set up in **Search &
Discovery**, when the section is set to *Products that go with it*. *Recently viewed*
reads a list stored in the visitor's own browser, and it is empty until that browser
has looked at another product.

Preview the store and click through a few products to see both fill up.

### My mega menu promo is not showing

Three things must all be true:

1. The menu runs **three levels deep** at that item in **Content → Menus** — the item,
   its children and their children. A two-level dropdown has no room for a promo.
2. The block's **Menu item title** matches the top-level menu item's title *exactly* —
   same spelling, same capitalization, no trailing space.
3. The block has an image or a heading.

Renaming a menu item in the admin does not rename it in the block.

### The Ingredients or Look inside button is missing on a product

The metafield is empty for that product, or the definition is not quite right. Check
[Tags and metafields](tags-and-metafields.md):

- Ingredients needs `custom.ingredients`, type **Multi-line text**.
- Look inside needs `custom.flipbook_pages`, type **File**, with **list of values**
  switched **on**. This is the one people miss — a single-file field will not work.

The buttons are hidden per product rather than shown empty, so you can add the block to
the template even when only some products carry the data.

### The personalization field is missing on a product

The product is not tagged. By default the block only shows on products tagged
`personalizable`. Either tag the product, or clear the block's **Only for products
tagged** setting to show the field on everything.

### The second photo does not appear on hover

Either the product has only one photo, or you are on a touch device. Phones and tablets
have no hover, so the rollover never triggers there — that is deliberate, and it means
phones do not download a second photo they can never show.

### The installment banner is not showing

Shop Pay Installments has to be available for your store, your currency and the
product's price. Where it does not apply, Shopify renders nothing and the theme shows
nothing rather than an empty box.

### Local pickup is not showing

It appears only when the selected *variant* is stocked at a location with local pickup
enabled. Check **Settings → Locations** and **Settings → Shipping and delivery → Local
pickup**, and check the variant's inventory at that location.

The location also needs a street address. Shopify lets you switch local pickup on for a
location that has only a country, but it does not offer pickup there, and the product
page shows nothing. Add the address under **Settings → Locations → [location] →
Address**, then save the location page itself.

### There are no filters on my collection page

Filters come from Shopify, not the theme. Install the free **Search & Discovery** app
and set them up under **Filters**. Until then the toolbar shows sorting only.

## Things that look wrong but are not

### The email popup opens whenever I select it in the theme editor

By design — you could not style it otherwise. It closes again when you select another
section. Its trigger and remembered dismissals only apply on the real storefront;
preview the store to see it behave normally.

### A visitor who closed my announcement bar sees it again

Changing the text of a message brings the bar back for everyone who had closed the old
one. A new announcement should be seen; an old dismissal should not silence it.

### My drop countdown shows a different time than I set

The launch time is read in the *visitor's* local time, not yours. `2026-08-01 18:00`
opens at six in the evening wherever the visitor happens to be. If you need one global
moment, say so in the section's copy.

Also: the countdown is a display, not a lock. Products stay reachable by their own URLs
while it counts down. To make them genuinely unbuyable, keep them unpublished until
launch.

### The custom cursor is not showing

It is off on touch devices and for visitors whose device is set to reduce motion. Both
are automatic and correct.

## Appearance

### My button labels are hard to read

**Theme settings → Colors →** the scheme in question **→ Text on accent**. That is the
color printed on an accent-filled button. A dark scheme with a bright accent needs a
dark value here; a light scheme with a deep accent needs a light one.

### The hairlines and dividers are invisible, or far too strong

They are mixed from **Text** and **Background** in each scheme. If they have gone
wrong, those two colors are too close together, or too far apart. The dimmest labels
are mixed the same way from **Muted text** and **Background** — if it is the small gray
labels that are hard to read, **Muted text** is the one to adjust.

### My headings do not look like the font I picked

Check the *weight* on the **Display font** setting — Shopify's font picker offers a
family and a weight, and the weight you pick is the weight your headings get. Some
families, especially display serifs, ship in one weight only.

### Product images look inconsistent in the grid

Set **Theme settings → Product cards → Image shape** to the shape your photography
actually uses, and shoot to it from then on. If your photos genuinely have different
shapes, turn on **Show full product image (no crop)** on the grid section — it fits
photos inside the card instead of cropping them.

### Images look soft or blurry

The theme requests images at the size it needs and serves smaller versions to smaller
screens. If they look soft, the uploaded file is too small. Upload product photos at
2000 px or more on the long edge; Shopify makes every smaller size from that.

## Settings and updates

### I added a new version and my colors are gone

An update you add from the notification under **Online Store → Themes** arrives as a
draft with your editor settings copied over. A theme added any other way — installed a
second time from the Theme Store, or uploaded as a file — is a separate theme that
starts from its style's own values. Add the update from the notification instead; see
[Getting started](getting-started.md#updating-to-a-newer-version-of-dolerite).

### I edited the theme and nothing changed on my store

Check which theme you edited. **Online Store → Themes** shows one theme as *Current
theme*; everything else is in the library and is not what visitors see. Editing an
unpublished theme is the right thing to do — you just have to publish it afterwards.

### Can I edit the code?

Yes, under **Online Store → Themes → ⋯ → Edit code**. Two things to know:

- Shopify carries code edits over to a new version only when they do not conflict with
  the update, and tells you on the theme's card whether it did. Note what you changed.
- Support covers the theme as shipped. We will always look at a problem and tell you
  what we find, but we cannot debug custom code or third-party app code for you.

Prefer a **Custom Liquid** section where one will do — it survives updates, because it
is a setting rather than an edit.
