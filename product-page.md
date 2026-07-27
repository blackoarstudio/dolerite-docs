---
title: "Product page"
description: "The blocks the Dolerite product page is built from, the media column, local pickup, gift cards and quick view."
---
# Product page

The product page is built from **blocks**. The media column on the left is fixed; the
information column on the right is yours to assemble — add the blocks you need, drag
them into the order you want, delete the ones you do not.

Open a product in the theme editor and click the **Product** section to see them.

## What ships by default

A new install places nine blocks, in this order:

1. Eyebrow
2. Title
3. Price
4. Description
5. Variant picker
6. Personalization field
7. Quantity
8. Stock status
9. Buy buttons

Everything else is available under **Add block**.

---

## The blocks

### Eyebrow

The small line above the title. **Text** chooses between the product's *type* (from
your admin) and *custom text* you type in.

### Vendor

The product's vendor. **Link to everything by this vendor** turns it into a link to
that vendor's products.

### Title

The product name. No settings.

### Price

Price, compare-at price and unit price. **Show tax and shipping note** adds a line
stating whether tax is included and linking to your shipping policy — on by default,
and expected in several markets.

When a product's variants have different prices, the price reads as a range starting
at the lowest.

### Stock status

A line saying whether the product is in stock, running low, or sold out — updated as
the visitor switches variants.

| Setting | Notes |
| --- | --- |
| **Call it low stock at or below** | 1–20, default 5. |
| **Show how many are left** | On by default. |

A number is only ever printed when Shopify tracks the inventory *and* the product
stops selling at zero. If a product is set to keep selling when out of stock, there is
no true remaining count, so the theme shows the state without inventing a figure.

### Description

The product description from your admin.

### Collapsible row

A titled row that opens and closes. Add as many as you need.

| Setting | Notes |
| --- | --- |
| **Heading** | The visible title. |
| **Text** | The content. |
| **Or take the text from a page** | Used when **Text** is empty. |

The page option is the useful one: write your returns policy on a page once, then add
a collapsible row pointing at it to every product. Editing the page updates every
product at once.

### Variant picker

The option selectors. One row per option, drawn automatically from the product.

Dolerite decides how to draw each option from the data you have:

1. **Swatch images or colors you set up in Shopify.** Under **Settings → Custom
   data → Metaobjects**, Shopify's swatch feature lets you attach a color or an image
   to an option value. If it is there, the theme uses it.
2. **Variant photos.** If every value of an option has its own photo and the photos
   actually differ, the theme uses those as image swatches.
3. **Text buttons.** Everything else — sizes, materials, lengths.

That order means "Color" gets swatches and "Size" gets buttons, without you setting
anything per product.

Values with no purchasable variant are marked as unavailable rather than hidden, so a
visitor can see that the combination exists and is sold out.

Selecting a variant swaps the gallery to that variant's photo, and swapping the
gallery back updates the selection. The URL updates too, so a shared link opens on the
right variant.

### Personalization field

An optional text field — a name, a date, a short message — that travels with the order
as a line item property and appears with the order in your admin.

| Setting | Notes |
| --- | --- |
| **Only for products tagged** | Default `personalizable`. Only products carrying this tag show the field. Clear the setting to show it on every product. |
| **Field label** | Also the name the value is filed under in the order. |
| **Max characters** | 5–100, default 30. |
| **Placeholder** | Example text inside the empty field. |
| **Example image marker** | See below. |

**Example image marker** connects the field to a photo. If any of the product's
gallery images has alt text *containing* this marker — the default is
`Personalization example` — a **Preview on product** button appears next to the field
and opens the zoom view on that one image. Set the alt text under **Products →
[product] → Media → Edit alt text**.

The field is deliberately optional. A customer who leaves it empty gets the product
without personalization.

### Quantity

A number field. It follows any quantity rules on the product — minimum, maximum and
increment — and re-reads them on every variant change, because a rule can differ from
one variant to the next.

### Buy buttons

The **Add to cart** button and, below it, Shopify's own express checkout buttons.

| Setting | Notes |
| --- | --- |
| **Show dynamic checkout buttons** | On by default. Shop Pay, PayPal, Google Pay — whichever your store has enabled under **Settings → Payments**. |
| **Show installment options** | On by default. Shows the Shop Pay Installments banner where it applies. |

This block also carries three things that attach themselves automatically:

- **Local pickup**, when the product's variant is stocked at a location that offers
  pickup. See below.
- **Gift card recipient fields**, when the product is a gift card. See below.
- The form itself. The quantity and personalization blocks attach to it wherever you
  drag them, so you can reorder freely.

### Ingredients button

Opens a panel with the product's ingredients text. Needs a metafield — see
[Tags and metafields](tags-and-metafields.md#ingredients). The button does not appear
on products where the metafield is empty.

### Look inside button

Opens a page-turn view of the product's flipbook images — for a book, a zine, a
catalogue or a lookbook. Needs a metafield — see
[Tags and metafields](tags-and-metafields.md#look-inside-flipbook).

### Text

A free rich-text block. Add as many as you like, anywhere in the stack.

### App blocks

Apps that support Online Store 2.0 add their own blocks here. Reviews under the price,
a subscription selector above the buy button, a size chart beside the variant picker —
you place them like any other block.

---

## The media column

The gallery on the left handles whatever media the product has:

- **Photos**, with a thumbnail strip. Clicking the main image opens a zoom view.
- **Video**, played in place.
- **3D models**, rotated by dragging. The 3D viewer is only downloaded when a product
  actually has a model.
- **Look inside**, when the flipbook metafield is set.

There is nothing to configure. Order the media under **Products → [product] →
Media**; the first item is the one that shows first.

## Local pickup

If a variant is stocked at a location with local pickup enabled, a line under the buy
buttons says so, and a link opens the list of stores with their availability and
pickup times.

Set this up under **Settings → Locations** and **Settings → Shipping and delivery →
Local pickup**. Nothing in the theme needs changing — availability is per variant, and
the theme re-checks it every time the visitor picks a different one.

## Gift cards

When the product is a gift card, the buy buttons block grows a set of recipient
fields: a checkbox to send it to someone else, then their email address, their name, a
message and an optional send date.

These fields only exist for gift card products. Create one under **Products → Add
product → This is a gift card**.

## The same blocks in two places

The **Featured product** section uses this identical block stack, so a featured
product on your home page behaves exactly like the product page. Two blocks are
product-page only — **Ingredients** and **Look inside** — because they open overlays
that belong to the product page's gallery.

## Quick view

Product cards across the store carry a quick-view button that opens the essentials —
media, options, price and add to cart — without leaving the page. It uses the same
option picker as the product page, so swatches and availability behave the same way.

There is no setting for it. Visitors who need the full page follow the card as usual.
