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

1. **Settings → Languages → Add language**.
2. Pick one of the six above and publish it.

The language picker appears in the footer as soon as your store has more than one
published language. You do not have to enable it anywhere.

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
