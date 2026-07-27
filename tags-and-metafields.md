---
title: "Tags and metafields"
description: "The five Dolerite features that read data from your products: badges, personalization, the example image, ingredients and the look-inside view."
---
# Tags and metafields

A handful of Dolerite's features read data from your products rather than from a
theme setting. That is deliberate: a badge or an ingredient list belongs to the
product, not to the page it happens to appear on, so setting it once in the admin
makes it correct everywhere at once.

There are five of them. None is required.

- [Product badges](#product-badges) — a tag
- [Personalization](#personalization) — a tag
- [The personalization example image](#the-personalization-example-image) — alt text
- [Ingredients](#ingredients) — a metafield
- [Look inside (flipbook)](#look-inside-flipbook) — a metafield

---

## Product badges

**Where:** Products → [product] → Tags

Tag a product `badge:` followed by the text you want, and that text appears as a badge
on the product card.

| Tag | Badge |
| --- | --- |
| `badge:Bestseller` | **Bestseller** |
| `badge:New in` | **New in** |
| `badge:Last pieces` | **Last pieces** |

The text is printed exactly as you type it, in whatever language you type it in. There
is no list of allowed values and nothing to translate — which is the point: you can
run a campaign badge for a weekend by tagging twenty products, and remove it by
untagging them.

Two badges are automatic and need no tag:

- **Sold out**, controlled by **Theme settings → Product cards → Mark sold-out
  products**.
- **Sale**, shown when a product has a compare-at price. **Show the discount as a
  percentage** turns it into "−30%".

Sold out and Sale never appear together — a sold-out product is sold out first.

---

## Personalization

**Where:** Products → [product] → Tags

The **Personalization field** block on the product page shows an optional text input:
a name, a date, a short dedication. It appears only on products carrying the tag named
in the block's **Only for products tagged** setting, which defaults to
`personalizable`.

So: tag the products that can be personalized `personalizable`, and only those show
the field.

Clear the setting entirely and every product shows it. Change it to any other word and
the theme looks for that word instead.

What the customer types travels with the order as a line item property. It shows on
the cart line, in the order in your admin, and on the packing slip — with the block's
**Field label** as its name. Name the field something you will still understand three
months later on a printed slip.

---

## The personalization example image

**Where:** Products → [product] → Media → Edit alt text

Customers want to see what personalization looks like before they buy it. If any of
the product's gallery images has alt text *containing* the marker in the block's
**Example image marker** setting — the default is `Personalization example` — a
**Preview on product** button appears next to the field and opens the zoom view on
that one image.

To set it up:

1. Upload a photo of a personalized version of the product.
2. Open **Media → Edit alt text** on that image.
3. Write alt text that describes the image *and* contains the marker, for example:
   `Leather tag engraved with a name — Personalization example`.

Alt text is read aloud by screen readers, so keep it a real description with the
marker appended, not the marker alone.

---

## Ingredients

**Where:** Settings → Custom data → Products

The **Ingredients button** block opens a panel with the product's ingredient list.

Create the metafield definition once:

| Field | Value |
| --- | --- |
| Namespace and key | `custom.ingredients` |
| Type | **Multi-line text** |

Then fill it in per product, at the bottom of the product page in the admin under
**Metafields**. Products where it is empty show no button — you can add the block to
the template safely even if only some products have the data.

Despite the name, this is just a long-text panel. Care instructions, technical
specifications, a materials list and allergen information all fit. If you rename it,
the button's label comes from your translations — see
[Translations and markets](translations-and-markets.md).

---

## Look inside (flipbook)

**Where:** Settings → Custom data → Products

The **Look inside button** block opens a page-turn view of a set of images — the right
tool for a book, a zine, a catalogue, a printed lookbook or a pattern.

Create the metafield definition once:

| Field | Value |
| --- | --- |
| Namespace and key | `custom.flipbook_pages` |
| Type | **File** |
| List of values | **On** — a single file is not enough |

The "list of values" switch is the part that is easy to miss. Without it the field
holds one file and the button will not appear.

Then, per product, add the page images **in reading order**. The order in the list is
the order they turn.

Products where the field is empty show no button.

---

## A note on metafield names

Both metafields use Shopify's `custom` namespace, which is the default one the admin
suggests. The keys — `ingredients` and `flipbook_pages` — must match exactly; the
theme looks for those names and nothing else. If you already have a metafield holding
this data under a different name, the quickest route is to create the definition above
and copy the values across.
