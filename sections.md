---
title: "Sections"
description: "All 22 sections you can add in the theme editor, plus the header, footer and the section behind every page type."
---
# Sections

A section is a band of content you add to a page in the theme editor. Dolerite has
**22 sections you can add anywhere**, grouped into five categories in the *Add
section* picker, plus the header, footer and page-specific sections described at the
bottom of this page.

Every section has a **Color scheme** setting and its own **Top padding** and **Bottom
padding** sliders, so they are not repeated in each entry below.

- [Products](#products)
- [Text](#text)
- [Media](#media)
- [Social proof](#social-proof)
- [Store](#store)
- [Header, footer and the two group sections](#header-footer-and-the-two-group-sections)
- [Page sections](#page-sections)

---

## Products

### Product grid

A row or grid of products from one collection. The workhorse of the home page.

| Setting | Notes |
| --- | --- |
| **Eyebrow**, **Heading** | The small label above the heading, and the heading. Leave either empty to hide it. |
| **Collection** | With none selected, the section renders placeholder cards so you can still see the layout. |
| **Products to show** | 2–12. |
| **Columns (desktop)** | 2–5. Phones follow **Products per row on phones** in theme settings. |
| **Show full product image (no crop)** | Off by default. On, photos are fitted inside the card instead of cropped to fill it — use it when your product photos have different shapes. |

### Featured product

One product, laid out large: media on one side, the full product block stack on the
other. Useful for a hero product on the home page or a landing page.

| Setting | Notes |
| --- | --- |
| **Product** | The product to show. |
| **Image position on desktop** | Left or right. |
| **Show thumbnail strip** | On by default. |
| **This is the first section on the page** | Turn on only when this section is the topmost one. It tells the browser to load the main image at top priority. Never turn it on for two sections on the same page. |

This section uses the same blocks as the product page — see
[Product page](product-page.md) for what each block does. It carries a slightly
shorter list: the ingredients and look-inside buttons are product-page only, because
they open overlays that only exist there.

### Collection teaser

A row of collections, each as a card with its image and name.

| Setting | Notes |
| --- | --- |
| **Collections** | Pick them in the order you want them shown. |
| **Collections to show** | 2–8. |
| **Columns on desktop** | 2–5. |
| **Show the number of products** | On by default. |
| **Load the first image immediately** | Off by default. Turn it on only when this section is the topmost one on the page. |
| **Link label**, **Link** | An optional link under the row, e.g. to your list of all collections. |

### Related products

Recommendations under a product. Only available on the product template.

| Setting | Notes |
| --- | --- |
| **Kind of recommendation** | *Similar products* uses Shopify's own recommendation engine and needs no setup. *Products that go with it* uses the complementary products you set up in Shopify's free **Search & Discovery** app — with none set up, that option shows nothing. |
| **Products to show** | 2–10. |
| **Columns on desktop** | 2–4. |

The row is fetched after the product page has loaded, so it never delays the product
itself. In the theme editor it stays empty — the editor has no visitor to recommend
for. Preview the storefront to see it.

### Recently viewed

The products this visitor has looked at, newest first. The current product is left
out.

| Setting | Notes |
| --- | --- |
| **Products to show** | 2–10. |
| **Columns on desktop** | 2–4. |

The list is stored in the visitor's own browser and never leaves it. A first-time
visitor sees nothing, and so does the theme editor — preview the storefront and click
through a few products to see it fill up.

### Drop

A timed release: before launch the grid is blurred and a countdown runs, at launch it
opens, and after an optional end time it closes again.

| Setting | Notes |
| --- | --- |
| **Eyebrow**, **Heading**, **Text** | The copy above the grid. |
| **Collection** | The products in the drop. |
| **Products to show** | 2–8. |
| **Columns (desktop)** | 2–4. |
| **Launch time** | Format `YYYY-MM-DD HH:MM`, in the visitor's local time. Leave empty for a drop that is already live. |
| **End time (optional)** | Same format. After it, the section shows the drop as ended. |

Both times are read in the *visitor's* local time, not yours. A drop set to
`2026-08-01 18:00` opens at six in the evening wherever the visitor is. This is
usually what you want for a worldwide release; if you need a single global moment,
say so in the copy.

The countdown is a display, not a lock. Products in the collection remain reachable by
their own URLs while the section is counting down. If a drop must be unbuyable before
launch, keep the products unpublished and publish them at launch.

---

## Text

### Rich text

A centered column of text. Blocks: **Eyebrow** (max 2), **Heading** (max 2, with a
size choice), **Text**, and **Buttons** (up to two buttons in one row). Up to 6
blocks. **Alignment** and **Column width** (480–960 px) are section settings.

### Editorial split

Text on one side, two overlapping images on the other. The section that carries a
brand story.

| Setting | Notes |
| --- | --- |
| **Eyebrow**, **Heading**, **Text** | The copy. |
| **Button label**, **Button link** | Optional. |
| **Large image**, **Small image** | The small one overlaps the large one. |
| **Media first (text right)** | Off by default. Turn on to mirror the layout. |

### Image with text

One image beside a column of blocks. More configurable than *Editorial split*, and
built for repeating down a page in alternating directions.

Section settings: **Image**, **Image position** (left/right), **Image width**
(narrow/half/wide), **Image shape** (adapt/wide/square/tall), **Vertical alignment**
(top/center/bottom).

Blocks, up to 6: **Eyebrow**, **Heading**, **Text**, **Checklist** (one item per
line), **Button** (up to two, solid or ghost).

*Image shape → adapt* keeps the image's own proportions. The other three crop it.

### Multicolumn

Two to five columns, each with an image, heading, text and an optional link. Use it
for "how it works", shipping promises or category shortcuts.

| Setting | Notes |
| --- | --- |
| **Columns on desktop** | 2–5. |
| **Text alignment** | Left or center. |
| **Number the columns** | Off by default. Turn on for a numbered process. |
| **Image shape** | Wide, square, tall or circle. |

Up to 8 column blocks.

### FAQ

Questions and answers as an accordion. Up to 20 question blocks, each with a
**Question** and a rich-text **Answer**. **Open first question by default** is on.

The accordion is built from the browser's own disclosure element, so it opens and
closes without JavaScript and reads correctly to a screen reader.

---

## Media

### Hero

The full-height opening section: eyebrow, heading, subheading, one button, and up to
four small **Marker** blocks (short phrases like "Free shipping" that sit under the
button).

| Setting | Notes |
| --- | --- |
| **Ambient accent glow** | On by default. A soft accent-colored light behind the text. |
| **Entrance animation** | On by default. |
| **Type the eyebrow line** | On by default. Types the eyebrow out character by character. |
| **Enable drive-by** | Off by default. Sends a small image travelling across the hero on a repeating cycle. **Custom mascot image** sets it, **Repeat cycle** the interval in seconds. |

All four motion settings stop automatically for visitors who prefer reduced motion.

### Slideshow

Up to 6 slides, each with an image, eyebrow, heading, text, a button, a content
position (left/center/right/bottom) and its own **Image darkening** value.

| Setting | Notes |
| --- | --- |
| **Name for screen readers** | What the slideshow is called to assistive technology, e.g. "Featured". |
| **Advance slides automatically** | Off by default. |
| **Seconds per slide** | 3–12. |
| **Height** | 40–90 % of the screen height. |
| **Full page width** | On by default. |

The slideshow scrolls: visitors swipe it on a phone the same way they swipe anything
else, and the arrow keys move it on a keyboard. When **Advance slides automatically**
is on, a pause button appears — autoplay without a way to stop it fails accessibility
requirements, so the button is not optional.

**Image darkening** is per slide because it depends on the photo. A bright image needs
more of it before white text is readable.

### Video

One video, either hosted by Shopify or embedded from YouTube or Vimeo.

| Setting | Notes |
| --- | --- |
| **Video** | A video uploaded to your Shopify files. Preferred — it plays without contacting another company's servers. |
| **Or a YouTube / Vimeo link** | Used when **Video** is empty. |
| **Cover image** | Shown before playback starts. For an external video this is what visitors see until they press play. |
| **Play muted on loop, without controls** | Off by default. Turns the video into a background element. |
| **Shape** | 16:9, 2.4:1 (cinematic), 1:1 or 9:16 (vertical). |
| **Full page width** | Off by default. |

An external video is not embedded until the visitor presses play. Until then the
section is just your cover image, which is why a good cover image matters here: it is
what most visitors will actually see.

---

## Social proof

### Testimonials

Up to 12 quote blocks: **Quote**, **Author**, **Detail** (role, city …) and a
**Stars** rating from 0 to 5, where 0 hides the stars.

The quotes that ship with the theme are placeholders. Replace them with real customer
feedback or remove the section — an invented review is still invented when a theme
supplies it.

### Logo list

A row of partner, press or payment logos. Up to 12 logo blocks: **Logo** image,
**Name** (used as the accessible label), **Caption** and an optional **Link**.

| Setting | Notes |
| --- | --- |
| **Logos per row** | 3–8. |
| **Logo height** | 24–80 px. |
| **Logo treatment** | *Plain* shows them in full color, *Mono* flattens them to one color, *Dim* fades them back. |

*Mono* is the safe default: press logos arrive in a dozen different colors and rarely
sit well together untouched.

### Trust badges

A row or stack of short promises — free delivery, easy returns, secure payment. Up to
6 badge blocks, each with an **Icon** chosen from thirteen built-in icons, or your own
image, plus a **Heading** and **Text**.

**Layout** switches between a row and a stack; **Draw a box around the row** adds a
panel behind it.

---

## Store

### Newsletter

An email signup that posts to your Shopify customer list.

| Setting | Notes |
| --- | --- |
| **Eyebrow**, **Heading**, **Text**, **Button label**, **Small print** | The copy. |
| **Layout** | *Center* stacks it; *split* puts the text and the field side by side. |
| **Draw a panel behind it** | On by default. |

Subscribers arrive under **Customers** in your admin with the tag `newsletter`, so you
can build a segment from them. The email popup tags its subscribers the same way, which
means one segment covers both.

### Email popup

The same signup, in an overlay. Add it once; it appears across the whole store.

| Setting | Notes |
| --- | --- |
| **Eyebrow**, **Heading**, **Text**, **Image**, **Button label**, **Small print** | The copy and an optional image. |
| **Trigger** | *After a delay* or *when the visitor moves to leave*. |
| **Delay** | 3–60 seconds, for the delay trigger. |
| **Show again after** | 1–90 days. How long a dismissal is remembered. |

The popup is always visible in the theme editor so you can style it. Dismissals are
only remembered on the real storefront.

Exit-intent works by watching the mouse leave the top of the window, which cannot
happen on a phone. On touch devices the exit trigger falls back to the delay.

### Contact form

Name, email, an optional phone number, and a message. Posts to the email address under
**Settings → Store details**.

| Setting | Notes |
| --- | --- |
| **Eyebrow**, **Heading**, **Intro text** | Optional copy above the form. |
| **Ask for a phone number** | Off by default. |

Your contact *page* already includes this section through the `page.contact` template.
Add the section separately only when you want a form somewhere else as well.

### Announcement bar

A thin bar above the header. Up to 5 message blocks, each with **Text**, an optional
**Link** and an optional **Icon** (truck, clock, gift, star, leaf or globe).

| Setting | Notes |
| --- | --- |
| **Style** | *Accent*, *Surface* or *Plain*. |
| **Let visitors close it** | On by default. |
| **Rotate between messages** | On by default. |
| **Seconds per message** | 3–12. |

With more than one message the bar rotates and shows arrows. Pressing an arrow stops
the rotation for that visit, so a visitor reading a long message is not moved on
mid-sentence.

Changing the text of a message brings the bar back for visitors who had closed the old
one — a new announcement should be seen.

This section lives in the header group and can only be added there.

### Custom Liquid

A field for your own Liquid, HTML or an app's embed code. **Constrain to page width**
is on by default; turn it off for something that should run edge to edge.

Use it for a third-party widget that has no app block. Code you paste here runs on your
storefront, so paste only code you trust and check the page afterwards — a syntax error
in this field affects the page it is on.

---

## Header, footer and the two group sections

The header and footer are sections too, but they live in *groups* — they appear on
every page, so they are edited once and cannot be added a second time.

### Header

| Setting | Notes |
| --- | --- |
| **Navigation menu** | Defaults to `main-menu`. |
| **Sticky header** | On by default. The header stays visible as the page scrolls. |
| **Show search icon** | On by default. |
| **Show account link** | On by default. Only appears when customer accounts are enabled under **Settings → Customer accounts**. |

Up to 4 **Mega menu promo** blocks — see
[Navigation and search](navigation.md#mega-menu-promos).

### Footer

| Setting | Notes |
| --- | --- |
| **Footer menu** | Defaults to `footer`. |
| **Credit line** | An optional line of text at the very bottom, beside the copyright. |

The footer also renders your social links (from **Theme settings → Social media**),
the payment icons Shopify reports for your store, and — when you sell in more than one
language or country — the language and country pickers. See
[Translations and markets](translations-and-markets.md).

---

## Page sections

Every page type has one section that renders it. You cannot add or remove these — the
template places them — but you can open each one in the editor and change its
settings. Most carry top and bottom padding; the ones with more are listed here.

| Page | Section | Settings beyond padding |
| --- | --- | --- |
| Product | **Product** | Built from blocks — see [Product page](product-page.md). |
| Collection | **Collection** | Show the collection image · Show the collection description · Columns (desktop) · Products per page |
| List of collections | **Collections** | Heading · Columns · Collections per page · Show product count |
| Search | **Search** | Results per page · Columns (desktop) |
| Blog | **Blog** | Columns · Posts per page · Show tag filter · and, for the article card: show image, image shape, excerpt, date, author |
| Article | **Article** | Show featured image · author · tags · previous and next post · Comments per page |
| Cart | **Cart** | — |
| Page | **Page** | — |
| 404 | **404** | — |
| Password | **Password** | Logo · Logo width · Heading · Show email signup · Show store owner link |
| Customer pages | **Login**, **Register**, **Account**, **Addresses**, **Order**, **Reset password**, **Activate account** | Heading and subheading on most; the order page can show or hide product images |

You *can* add ordinary sections above and below these on any template — a **Trust
badges** row under the cart, an **FAQ** under the product, a **Newsletter** at the
bottom of the collection page. That is the point of Online Store 2.0, and Dolerite's
sections are built to sit anywhere.
