---
title: "Getting started"
description: "Install Dolerite, work through the setup checklist, and publish. Also: how to move to a newer version of the theme."
---
# Getting started

## 1. Install the theme

1. On Dolerite's page in the Shopify Theme Store, pick the style you want to start
   from — **Dolerite**, **Alabaster** or **Anthracite** — and add the theme to your
   store.
2. In your Shopify admin, go to **Online Store → Themes**. The theme is waiting among
   your draft themes.
3. Open it in the theme editor. The theme is not live yet — visitors still see your
   current theme until you publish.

You can set the theme up and preview it before you buy it. Shopify asks for the purchase
when you publish.

The three styles are starting points, not three themes. A style sets the colors, the
fonts and a handful of layout options, and it installs its own home page. Everything a
style sets can be changed afterwards.

Work through the rest of this page before you publish. Everything below is reversible.

## 2. What ships on the home page

Each style installs the home page of its demo store:

| Style | Home page sections, in order |
| --- | --- |
| **Dolerite** | Hero, Product grid, Editorial split, Slideshow, Collection teaser |
| **Alabaster** | Hero, Slideshow, Product grid, Editorial split, Collection teaser |
| **Anthracite** | Hero, Video, Product grid, Slideshow, Editorial split, Featured product, Drop, Collection teaser |

All three start with an announcement bar above the header. Anthracite also installs a
newsletter sign-up and three columns in the footer, four collapsible rows and an
**Image with text** section on the product page, and a second product template,
`product.gift-card`, meant for a gift card product.

**The text is example copy from the demo store, not yours.** It names products you do
not sell and makes promises you have not made: free shipping above an amount, a
guarantee of so many years, a returns window, a drop on a certain day. Replace all of
it before you publish — step 4 lists where it sits.

What you see until you add your own content:

- **Product grid** shows the first eight products of your catalog. In a store without
  products it shows gray placeholder cards.
- **Slideshow**, **Editorial split** and **Collection teaser** show placeholder artwork
  until you choose images and collections.
- On Anthracite, **Video** shows a play button over Shopify's sample video until you
  upload your own, **Featured product** shows a placeholder title and price until you
  pick a product, and **Drop** shows blurred placeholder cards under a countdown until
  you choose a collection and set your own launch time.

None of that is an error. It is the theme telling you a setting is still empty.

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

Footer columns can each list a menu of their own. Anthracite installs two, set to the
same two menus; point them at menus you build for the footer.

A top-level item whose menu runs **three levels deep** — the item, its children and
their children — opens as a mega menu. See [Navigation and search](navigation.md).

### Colors

Theme editor → **Theme settings → Colors**.

Four color schemes ship with the theme. **Page color scheme** decides which one paints
the page itself: the header, the cart drawer and the sections behind each page type —
collection, product, cart, search and the rest — which have no color setting of their
own.

The sections you add, and the footer, each have a **Color scheme** setting that starts
on Scheme 1. A section on the same scheme as the page blends into it; a section on any
other scheme stands out as a band of color. If you move **Page color scheme** off
Scheme 1, the sections still set to Scheme 1 keep it and turn into bands — switch them
too. Read
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

The **Product grid** on the home page starts on all products. Open it and choose the
**Collection** you want to feature. Set **Products to show** and **Columns (desktop)**
to taste. Pick the collections for the **Collection teaser** in the same pass.

### Pages every store needs

Create these under **Content → Pages**, then link them from the footer menu:

- A contact page. Create the page, and in **Theme template** choose `page.contact` —
  that template renders a working contact form.
- Your policies. Shopify generates refund, privacy, terms and shipping policies under
  **Settings → Policies**; they get their own URLs and belong in the footer menu.

### Cart style

Theme editor → **Theme settings → Cart**. **Let customers add a note to their order**
shows a note field in both the cart drawer and the cart page. It is on in the Dolerite
and Alabaster styles and off in Anthracite.

## 4. Replace the example text

None of the text the theme installs with should survive to your live store. Work
through it in this order:

1. **The home page**, section by section — headings, paragraphs, button labels and the
   three short lines under the hero button.
2. **The announcement bar.** It starts with a free shipping message; Anthracite adds a
   message about a drop and one about a guarantee.
3. **On Anthracite, the product page and the footer.** The four collapsible rows
   describe materials, shipping, returns and a guarantee, and they appear on every
   product. The footer carries a line about the shop and a newsletter invitation.

Sections you add yourself start with short default text. Most of it describes what
belongs in that spot; some of it makes an offer — the email popup's default heading
promises 10% off a first order, the announcement bar's default message free delivery.
Keep an offer only if it is true.

If you add the **Testimonials** section, its quotes are placeholders. Replace them with
real customer feedback or remove the section. Never publish an invented review.

## 5. Preview and publish

1. In the theme editor, use the device icons to check phone and tablet widths.
2. Close the editor and choose **Actions → Preview** to click through the real store:
   home → collection → product → cart.
3. When you are happy, **Actions → Publish**.

## Updating to a newer version of Dolerite

When a new version is released, a notification replaces the theme's version number
under **Online Store → Themes**.

1. Click the notification and choose **Add to draft themes**. Shopify adds the new
   version as a draft and copies over what you did in the theme editor: settings,
   sections, templates, app blocks and wording.
2. Check the draft. The editor lets you work on it without visitors seeing it.
3. Publish when it matches.

Keep the old version for a week or two before removing it. If you edited theme code,
Shopify carries the edits over when they do not conflict with the update, and the
theme's card says whether they were included — check there before you publish.
