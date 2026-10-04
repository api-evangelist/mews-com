---
title: "TikTok Pixel attribution breaks across Mews iframe checkout — anyone solved this?"
url: "https://community.mews.com/t/tiktok-pixel-attribution-breaks-across-mews-iframe-checkout-anyone-solved-this/2366#post_3"
date: "2026-09-25"
author: "@william.diprimo william.diprimo"
feed_url: "https://community.mews.com/posts.rss"
---
Yes, this is a known challenge with cross-domain tracking when the Booking Engine confirmation page loads on app.mews.com . Mews supports adding a GTM container to the Booking Engine, but TikTok Pixel and other third-party tags must be configured within that container by the property or its marketing partner. The usual workaround is to persist the TikTok click identifier and relevant cookie/session values before the domain transition, then restore them for the Purchase event using custom GTM/JavaScript.
