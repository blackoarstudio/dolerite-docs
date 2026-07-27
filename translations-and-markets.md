---
title: "Translations and markets"
description: "The six languages Dolerite ships with, how to add another, selling in more than one country, and what is not translated."
---
# Translations and markets

## Languages included

Dolerite ships translated storefront text in six languages:

English (default) · German · French · Spanish · Italian · Thai

That covers every word the *theme* says — "Add to cart", "Sold out", "Filter",
"Continue shopping", error messages, form labels, everything. Your own content —
product names, descriptions, page copy, menu items — is translated separately, by you.

## Adding a language

It takes three steps, and the first two on their own change nothing on your
storefront. This catches almost everybody.

1. **Settings → Languages → Add language**. Pick one of the six above.
2. **Publish it** — from the `…` menu next to the language. An unpublished language
   does not exist as far as your storefront is concerned. Shopify will warn you that
   you have no translations yet; publish anyway. That warning is about *your* content
   (products, pages), and the theme's own text is already translated.
3. **Settings → Markets → your market → Domains and languages** — add the language
   there too. **This is the step people miss.** Until a language is switched on for
   the market a visitor is browsing, the storefront stays in your default language
   and no picker appears.

The language picker appears in the footer once all three are done, and only then.
If you have finished step 2 and see no picker, step 3 is why.

### About the URL

Step 3 asks you to set up a subfolder, and it offers to give **every** language one —
including your main language, which would move your whole store from `example.com/`
to `example.com/en-us/`. That is a real change to every URL you have.

Unless you want that, remove the suffix from your primary language in that dialog.
The main language then stays at the root and only the added language gets a folder,
which is what most stores want.

To translate your own product and page content, use Shopify's free **Translate &
Adapt** app, or any translation app from the App Store.

### A language that is not in the list

You can publish any language Shopify supports. The theme's own text will fall back to
English until it is translated. To translate it:

**Online Store → Themes → [Dolerite] → ⋯ → Edit default theme content**

That screen lists every phrase the theme uses, per language, and lets you type your
own. Nothing needs to be edited in code.

## Selling in more than one country

If you have set up markets under **Settings → Markets**, a country picker appears in
the footer next to the language picker. Choosing a country switches the currency and
the prices for that market.

Language and country are two separate pickers on purpose. They are not the same
question — a customer in Belgium may want French prices in euros, and a customer in
Switzerland may want German prices in francs.

Prices are formatted the way the visitor's locale writes numbers, so a German visitor
sees `1.299,00 €` and an English one `€1,299.00`, from the same underlying price.

## What is not translated, and why

**Text you type into theme settings is not translated.** Your hero heading, your FAQ
answers, your trust badge captions, your announcement bar messages — those are your
words, stored once. To show different words in a different language, use **Translate &
Adapt**, which can translate theme settings as well as products and pages.

**Product badges from tags are not translated.** A product tagged `badge:Bestseller`
shows "Bestseller" in every language. That is the trade-off for badges you can set up
in seconds without touching a translation file. If you need a translated badge, use a
tag in the language most of your customers read, or leave badges off in that market.

## Checking a translation before you publish

Add `?locale=de` to any storefront URL to preview it in a published language — for
example `https://your-store.com/collections/all?locale=de`. Use it to walk one full
path per language: home → collection → product → cart.

Thai is worth a specific look. It sets taller than Latin scripts, so check that
buttons and card titles still fit the layout you chose.
