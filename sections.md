---
title: "Sections"
description: "All 22 sections you can add in the theme editor, plus the header, footer and the section behind every page type."
---
# Sections

A section is a band of content you add to a page in the theme editor. Dolerite has
**22 sections you can add**, grouped into five categories in the *Add section* picker,
plus the header, footer and page-specific sections described at the bottom of this
page. Nineteen of them can go on any page. Three have a fixed place: **Announcement
bar** only in the header area, **Email popup** only in the footer area, and **Related
products** only on the product page.

The sections you add have a **Color scheme** setting and their own **Top padding** and
**Bottom padding** sliders, so those are not repeated in each entry below. The two
overlays, **Announcement bar** and **Email popup**, have no padding. Many sections also
have an **Eyebrow** — the small label above the heading — and a **Heading**; leave
either empty to hide it.

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
| **Columns (desktop)** | 2–4. Phones follow **Products per row on phones** in theme settings. |
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

Until a product is picked, the section shows a placeholder image with a placeholder
title and price, and in the theme editor a note asking you to pick one.

This section uses the same blocks as the product page — see
[Product page](product-page.md) for what each block does. It carries a slightly
shorter list: the ingredients and look-inside buttons are product-page only, because
they open overlays that only exist there.

### Collection teaser

A row of collections, each as a card with its image and name.

| Setting | Notes |
| --- | --- |
| **Eyebrow**, **Heading** | The copy above the row. |
| **Collections** | Pick them in the order you want them shown. With none picked, the row shows placeholder tiles — as many as **Collections to show**. |
| **Collections to show** | 2–12. |
| **Columns on desktop** | 2–4. |
| **Show the number of products** | On by default. |
| **Load the first image immediately** | Off by default. Turn it on only when this section is the topmost one on the page. |
| **Link label**, **Link** | A button beside the heading, e.g. to your list of all collections. With **Link** empty it goes there on its own. The button needs an eyebrow or a heading to sit beside; with both empty it is not shown. |

### Related products

Recommendations under a product. Only available on the product template.

| Setting | Notes |
| --- | --- |
| **Kind of recommendation** | *Similar products* uses Shopify's own recommendation engine and needs no setup. *Products that go with it* uses the complementary products you set up in Shopify's free **Search & Discovery** app — with none set up, that option shows nothing. |
| **Products to show** | 2–10. |
| **Columns on desktop** | 2–4. |

The row is fetched after the product page has loaded, so it never delays the product
itself. A product Shopify has no recommendations for shows nothing at all — the section
stays out of the way rather than printing an empty heading.

### Recently viewed

The products this visitor has looked at, newest first. The current product is left
out.

| Setting | Notes |
| --- | --- |
| **Products to show** | 2–10. |
| **Columns on desktop** | 2–4. |

The list is stored in the visitor's own browser and never leaves it. A first-time
visitor sees nothing. To see it fill up, click through a few products in the preview.

### Drop

A timed release: before launch the grid is blurred and a countdown runs, at launch it
opens, and after an optional end time it closes again.

| Setting | Notes |
| --- | --- |
| **Eyebrow**, **Heading**, **Text** | The copy above the grid. |
| **Collection** | The products in the drop. With none chosen, the grid shows four placeholder cards. |
| **Products to show** | 2–12. |
| **Columns (desktop)** | 2–5. |
| **Launch time** | Format `YYYY-MM-DD HH:MM`, in the visitor's local time. Leave empty for a drop that is already live. |
| **End time (optional)** | Same format. After it, the section shows the drop as ended. |

Both times are read in the *visitor's* local time, not yours. A drop set to
`2026-08-01 18:00` opens at six in the evening wherever the visitor is. This is
usually what you want for a worldwide release; if you need a single global moment,
say so in the copy.

While the drop is locked, the cards in the grid cannot be clicked or reached with the
keyboard. With an end time set, the countdown switches to the time remaining once the
drop is live; after the end the grid is grayed out and can no longer be clicked.

The countdown is a display, not a lock. Products in the collection remain reachable by
their own URLs while the section is counting down. If a drop must be unbuyable before
launch, keep the products unpublished and publish them at launch.

---

## Text

### Rich text

A centered column of text. Blocks: **Eyebrow** (max 2), **Heading** (max 2, with a
size choice), **Text**, and **Buttons** (up to two buttons in one row). Up to 6
blocks. **Alignment** and **Column width** (480–1000 px) are section settings.

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

Section settings: **Image**, **Image position** (Left / Right), **Image width**
(Narrow / Half / Wide), **Image shape** (Adapt to image / Landscape (16:10) /
Square (1:1) / Portrait (4:5)), **Vertical alignment** (Top / Middle / Bottom).

Blocks, up to 6: **Eyebrow**, **Heading**, **Text**, **Checklist** (one item per
line), **Button** (up to two, **Solid** or **Outline**).

*Image shape → Adapt to image* keeps the image's own proportions. The other three crop
it.

### Multicolumn

Two to four columns, each with an image, heading, text and an optional link. Use it
for "how it works", shipping promises or category shortcuts.

| Setting | Notes |
| --- | --- |
| **Columns on desktop** | 2–4. |
| **Text alignment** | Left or center. |
| **Number the columns** | Off by default. Turn on for a numbered process. |
| **Image shape** | Landscape (16:10), Square (1:1), Portrait (4:5) or Circle. |

Up to 8 column blocks. A column's link is its **Link label** and **Link**.

### FAQ

Questions and answers as an accordion. Up to 20 question blocks, each with a
**Question** and a rich-text **Answer**. **Open first question by default** is on.

The accordion is built from the browser's own disclosure element, so it opens and
closes without JavaScript and reads correctly to a screen reader.

---

## Media

### Hero

The opening section: eyebrow, heading, subheading, one button, and up to
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

Up to 6 slides, each with an image, eyebrow, heading, text, a button, a **Content
position** (Left / Center / Right / Bottom left) and its own **Image darkening** value.
A slide without an image shows placeholder artwork.

| Setting | Notes |
| --- | --- |
| **Name for screen readers** | What the slideshow is called to assistive technology, e.g. "Featured". |
| **Advance slides automatically** | Off by default. |
| **Seconds per slide** | 3–12. |
| **Height** | 40–90 % of the screen height. With **Show the whole image**, the tallest an image may grow on a wide screen. |
| **Image fit** | **Fill the slide** (default) or **Show the whole image**. See below. |
| **Full page width** | On by default. |

**Image fit** decides what happens when a photo and a slide have different shapes — and
they always do, because the slide is as wide as the window. **Fill the slide** covers
the slide with the image and crops whatever does not fit: on a wide desktop that is the
top and bottom, on a phone the sides. It suits atmosphere shots where no edge matters.
**Show the whole image** never crops. The image keeps its own shape and stands beside
the text on wide screens and above it on screens up to 900 px; the text is no longer on
the photo, so **Image darkening** has nothing to do in this mode. Use it when the photo
shows a product that has to be seen whole.

The slideshow scrolls: visitors swipe it on a phone the same way they swipe anything
else. With more than one slide it shows arrows and dots, and both work from the
keyboard. When **Advance slides automatically**
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
| **Cover image** | For a YouTube or Vimeo video: what visitors see until they press play. An uploaded video shows its own first frame instead. |
| **Play muted on loop, without controls** | Off by default. For an uploaded video only: turns it into a silent background loop, paused for visitors who prefer reduced motion. With a YouTube or Vimeo link the switch does nothing. |
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
| **Logos per row** | 2–6. |
| **Logo height** | 24–96 px. |
| **Logo treatment** | **As uploaded** shows them in full color, **Monochrome** flattens them to one color, **Dimmed until hover** fades them back until the pointer is on them. |

**Monochrome** is the default, and the safe one: press logos arrive in a dozen
different colors and rarely sit well together untouched.

### Trust badges

A row or stack of short promises — free delivery, easy returns, secure payment. Up to
6 badge blocks, each with an **Icon** chosen from thirteen built-in icons, or an image
of your own under **Or your own icon**, plus a **Heading** and **Text**.

**Small heading** puts a short label above the badges. **Layout** switches between
**Side by side** and **Stacked**; **Draw a box around the row** adds a panel behind it.

---

## Store

### Newsletter

An email signup that posts to your Shopify customer list.

| Setting | Notes |
| --- | --- |
| **Eyebrow**, **Heading**, **Text**, **Button label**, **Small print** | The copy. |
| **Layout** | **Centered** stacks it; **Text and field side by side** does what it says. |
| **Draw a panel behind it** | On by default. |

Subscribers arrive under **Customers** in your admin with the tag `newsletter`, so you
can build a segment from them. The email popup tags its subscribers the same way, which
means one segment covers both.

### Email popup

The same signup, in an overlay. It can only be added in the footer area of the editor;
add it once there and it appears across the whole store.

| Setting | Notes |
| --- | --- |
| **Eyebrow**, **Heading**, **Text**, **Image**, **Button label**, **Small print** | The copy and an optional image. |
| **Trigger** | *After a delay* or *when the visitor moves to leave*. |
| **Delay** | 2–60 seconds, for the delay trigger. |
| **Show again after** | 0–90 days. How long a dismissal is remembered. 0 means a visitor who closed it never sees it again. |

In the theme editor the popup opens while its section is selected, so you can style it,
and closes when you select something else. Dismissals are only remembered on the real
storefront.

Exit-intent works by watching the mouse leave the top of the window, which cannot
happen on a phone. On touch devices the exit trigger falls back to the delay.

### Contact form

Name, email, an optional phone number, and a message. Posts to the email address under
**Settings → Store details**.

| Setting | Notes |
| --- | --- |
| **Eyebrow**, **Heading**, **Intro text** | The copy above the form. Left empty, each shows the theme's own translated wording instead of disappearing. |
| **Ask for a phone number** | Off by default. |

Your contact *page* already includes this section through the `page.contact` template.
Add the section separately only when you want a form somewhere else as well. A page
takes one contact form.

### Announcement bar

A thin bar above the header. Up to 5 message blocks, each with **Text**, an optional
**Link** and an optional **Icon** (Delivery, Time, Gifting, Quality, Sustainability or
Worldwide).

| Setting | Notes |
| --- | --- |
| **Style** | **Accent color**, **Panel** or **Plain**. |
| **Let visitors close it** | On by default. |
| **Rotate between messages** | On by default. |
| **Seconds per message** | 3–15. |

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
| **Show account** | On by default. Shopify's account button: visitors sign in from a sheet without leaving the page, signed-in customers get their account menu. Only appears when customer accounts are enabled under **Settings → Customer accounts**. |

Up to 4 **Mega menu promo** blocks — see
[Navigation and search](navigation.md#mega-menu-promos).

### Footer

| Setting | Notes |
| --- | --- |
| **Footer menu** | Defaults to `footer`. The short line of links at the very bottom — the usual place for privacy, terms and contact. |
| **Show Follow on Shop button** | On by default. Lets customers follow your store in the Shop app. Shows once the Shop channel is installed and Shop Pay is active. |
| **Show payment icons** | On by default. The payment methods your store accepts, as Shopify reports them. Nothing is shown until a payment provider is set up. |
| **Credit line** | An optional line of text at the very bottom, beside the copyright. |

Up to 4 column blocks sit above that line:

- **Text column** — a heading and a short paragraph about the shop.
- **Menu column** — a heading and a menu of its own. Add one per menu you want to list.

Without any column blocks the footer is a single line. That is how the Dolerite and
Alabaster styles install; Anthracite installs with a text column, two menu columns and
a newsletter sign-up above them.

To put a newsletter sign-up above the footer on every page, add the **Newsletter**
section to the footer area in the editor instead of to a single page.

The footer also renders your social links (from **Theme settings → Social media**)
and — when you sell in more than one language or country — the language and country
pickers. See [Translations and markets](translations-and-markets.md).

---

## Page sections

Every page type has one section that renders it. You cannot add or remove these — the
template places them — but you can open each one in the editor and change its
settings. Most carry top and bottom padding; the ones with more are listed here.

| Page | Section | Settings beyond padding |
| --- | --- | --- |
| Product | **Product** | Built from blocks — see [Product page](product-page.md). |
| Collection | **Collection** | Show the collection image · Show the collection description · Columns (desktop) · Products per page |
| List of collections | **Collections** | Heading · Columns (desktop) · Collections per page · Show product count |
| Search | **Search** | Results per page · Columns (desktop) |
| Blog | **Blog** | Columns (desktop) · Posts per page · Show tag filter · and, for the article card: show featured image, image shape, excerpt, date, author |
| Article | **Article** | Show featured image · author · tags · previous and next post · Comments per page |
| Cart | **Cart** | — |
| Page | **Page** | — |
| 404 | **404** | — |
| Password | **Password** | Logo · Logo width · Heading · Show email signup · Show store owner link |
| Customer pages | **Login**, **Register**, **Account**, **Addresses**, **Order**, **Reset password**, **Activate account** | Heading and subheading on most; the order page can show or hide product images |

You *can* add ordinary sections above and below these on any template — a **Trust
badges** row under the cart, an **FAQ** under the product, a **Newsletter** at the
bottom of the collection page. That is the point of Online Store 2.0, and apart from
the three with a fixed place, Dolerite's sections are built to sit anywhere.
