# Add2Cart

Add2Cart is a React/Vite marketplace demo. It keeps catalog edits, cart contents, saved items, delivery addresses, and purchase history in the shopper's browser using localStorage. No account or server API is required.

## Run locally

```sh
npm install
npm run dev
```

Vite runs the storefront locally. Use `npm run build` to create the production static site, `npm run preview` to preview that build, and `npm run lint` to check the source.

## Guest shopping

Shoppers can browse, search, filter categories, save items, add to cart, and use Buy Now without signing in. Cart quantities and inventory are kept in this browser. Checkout collects a delivery address and payment choice, then records a demo order locally. Cash on delivery and e-wallet are display options only; the app does not collect payments. Saved delivery addresses and order history are also stored in this browser and are not shared between devices.

My products is a local listing manager. Listings are stored with the catalog in this browser and are not published to a shared marketplace.

## Existing database data

The former SQLite API source files were removed as part of the authentication removal. Existing files under `server/data` are intentionally left untouched; the storefront no longer reads or writes them. Back up that directory before manually removing any old database or uploaded files.
