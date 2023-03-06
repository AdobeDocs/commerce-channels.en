---
title: Price Scope
description: Use the Commerce pricing scope to manage pricing according to multiple websites or globally.
exl-id: 24a1eac1-d579-4063-a33c-71969bc2b4b9
---
# Price Scope

[!DNL Commerce] provides configuration for your [pricing scope](https://docs.magento.com/user-guide/configuration/catalog/catalog.html#price){target="_blank"} to be set to `Global` or `Website`. If pricing is set to `Global`, there is a single price source for all websites. If pricing is set to `Website`, your websites can vary their pricing across and also have a fallback default pricing value. See [Catalog Price](https://docs.magento.com/user-guide/configuration/catalog/catalog.html#price){target="_blank"} in the core Commerce user guide.

If you change your catalog price scope from `Global` to `Website`, all price type attributes also change to `Website`. See [Adding Websites](https://docs.magento.com/user-guide/stores/stores-all-create-website.html){target="_blank"}.

When a website price is chosen, there are two price sources:

- The website price
- The default (fall back) price

For the Amazon sales channel integration, based on your [listing rules](./listing-rules.md), you can map products from multiple websites into a single [!DNL Amazon Marketplace] Country (defined during [store integration](./store-integration.md)). However, this mapping introduces the issue of which price should be published if the product exists on multiple websites with differing prices.
