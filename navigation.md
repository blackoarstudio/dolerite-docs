---
title: "Navigation and search"
description: "Menus, dropdowns and mega menus with promos, mobile navigation, search, filters and sorting, breadcrumbs and the cart drawer."
---
# Navigation and search

## Menus

Menus are built in your Shopify admin under **Content → Menus**, not in the theme.
Dolerite reads two of them, and both are pre-selected:

| Menu handle | Where it appears | Setting |
| --- | --- | --- |
| `main-menu` | Header, and the mobile drawer | Header section → **Navigation menu** |
| `footer` | Footer | Footer section → **Footer menu** |

To use a different menu, build it in the admin and pick it in the section setting.

## Dropdowns and mega menus

How a menu item behaves in the header depends on how deep it goes:

| Menu structure | Result |
| --- | --- |
| A top-level item with no children | A plain link. |
| A top-level item with children | A dropdown list. |
| A top-level item with children that themselves have children | A **mega menu**: the second level becomes column headings, the third level becomes the links under them. |

So a mega menu is not a setting — it is what you get by building three levels in the
admin. For example:

```
Shop                        ← top level
├─ Apparel                  ← becomes a column heading
│  ├─ T-shirts              ← becomes a link in that column
│  ├─ Knitwear
│  └─ Outerwear
├─ Accessories              ← second column
│  ├─ Bags
│  └─ Caps
└─ Home                     ← third column
   ├─ Ceramics
   └─ Textiles
```

Each column heading is itself a link, so "Apparel" stays clickable.

### Mega menu promos

A mega menu can carry an image promo on its right-hand side. Add a **Mega menu promo**
block to the Header section — up to four.

| Setting | Notes |
| --- | --- |
| **Menu item title** | The *exact* title of the top-level menu item whose mega menu should show this promo. |
| **Image** | Shown as a square. |
| **Heading** | The label under the image. |
| **Link** | Where the promo goes. |

**Menu item title** is matched literally against the menu item's title. If the promo
does not appear, check for a trailing space or a different capitalization, and check
that the menu item actually has three levels — a two-level dropdown has no room for a
promo.

Rename a menu item in the admin and you must rename it in the promo block too.

## Mobile navigation

On phones the menu collapses into a drawer behind the burger icon. It is built from
the same `main-menu`, with sub-items nested inside expandable rows. There is nothing
to configure.

## Search

The header's search icon opens a search overlay. As the visitor types, results appear
below the field: matching products with their photo and price, plus collections,
pages and articles.

Pressing enter goes to the full search page, which has the same filtering and sorting
toolbar as a collection page.

Search matches from the beginning of words, which is what shoppers expect — typing
"jack" finds "jacket".

To improve results, use Shopify's free **Search & Discovery** app: it lets you add
synonyms ("trainers" → "sneakers"), boost particular products, and set up the filters
described below.

## Filters and sorting

Collection and search pages share one toolbar: filters on the left, a sort dropdown on
the right.

**Filters come from Shopify, not from the theme.** Set them up in **Search &
Discovery → Filters** — availability, price, and any product option, tag or metafield
you choose to expose. Whatever you enable there appears in the toolbar; enable none
and the toolbar shows only sorting.

Sorting options are Shopify's standard set — featured, best selling, alphabetical,
price, date. The collection's own default sort order, set under **Products →
Collections → [collection]**, is what a visitor sees before they choose anything.

Filters and sorting are both plain links and a plain form, so they work with
JavaScript disabled and each filtered view has its own URL a customer can share or
bookmark.

## Breadcrumbs

A breadcrumb trail appears under the header on collection, product, blog, article,
page and search pages. It is generated automatically and marked up so search engines
can read it. There is nothing to configure.

On a product page the trail shows the collection the visitor arrived through. Reaching
a product directly — from a search result or a shared link — gives a shorter trail,
because there is no collection to name.

## The cart drawer

Adding to cart opens a drawer rather than sending the visitor to the cart page. It
shows line items, quantities, the note field (if enabled in **Theme settings → Cart**),
the subtotal and a checkout button.

The cart page still exists at `/cart` and is fully built — the footer and the drawer
both link to it — because some customers prefer a full page, and because the express
checkout buttons belong there.
