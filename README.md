# Terra a Mar — Shopify Theme

The official Shopify theme for Terra a Mar, built on top of [Shopify Horizon](https://github.com/Shopify/horizon) (v4.2.0), Shopify's first-party Online Store 2.0 theme.

## Project status

- [x] Horizon base theme imported and rebranded (`theme_info` in `config/settings_schema.json`).
- [ ] Brand design (`terr.a.mar.dc.html` Claude Design project) imported: content, imagery, color palette, typography, and custom sections/templates matching the approved design.
- [ ] Store assets (`assets/logo-terramar.svg`, `assets/pieces/*.jpg`) added.

Until the design import lands, the theme runs with Horizon's stock structure, sections, and neutral default styling — it is fully installable and functional on a Shopify store, but not yet visually branded.

## Getting started

Install the [Shopify CLI](https://shopify.dev/docs/storefronts/themes/tools/cli), then from this directory:

```sh
shopify theme dev --store <your-store>.myshopify.com
```

This starts a local development server with hot reload against a real (or development) store.

To push this theme to a store:

```sh
shopify theme push --store <your-store>.myshopify.com
```

### Theme Check

Lint the theme with [Theme Check](https://shopify.dev/docs/storefronts/themes/tools/theme-check):

```sh
shopify theme check
```

## Staying up to date with Horizon

This theme keeps track of its base with an `upstream` remote pointing at Shopify's Horizon repository, so improvements/fixes from Horizon can be merged in later:

```sh
git remote add upstream https://github.com/Shopify/horizon.git
git fetch upstream
git merge upstream/main
```

## License

This theme is derived from Shopify Horizon, Copyright (c) 2025-present Shopify Inc. — see [LICENSE.md](/LICENSE.md). Per that license, this derived theme may be used for Terra a Mar's own Shopify store, but may not be resold, relicensed, redistributed, or listed on the Shopify Theme Store or any other marketplace.
