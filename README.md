# Mer Tun

A trilingual website for buying and renting real estate across Armenia.

## Files

- `index.html`: semantic page structure.
- `style.css`: responsive cream and forest-green visual design.
- `script.js`: fictional listings, search filters, sorting, details dialog, saved homes and translations.
- `images/`: local AI-generated concept imagery and SVG favicon.

## Run

Extract the project folder and open `index.html` in a modern browser. No installation or build step is required. You can also serve this folder with any static web server.

English is the default language. The language selector switches all interface copy and listing descriptions to Armenian or Russian. Browser local storage remembers the selected language and saved properties on this device. The site remains usable when local storage is unavailable. Filter values are preserved when changing languages.

## Features

- Buy and rent modes; all ten Armenian regions and Yerevan.
- Region, town, property type, maximum AMD price, room count and minimum area filters.
- Sorting by price and area; load more results; empty state and reset.
- Accessible property details dialog, keyboard focus and responsive layout.
- Local saved-property toggles.

## Publish on GitHub Pages

1. In `viktoria-voskanyan/armenia-homes`, choose **Add file → Upload files**.
2. Upload the contents of this folder (not the ZIP itself). `index.html` must be at the repository root. Keep `images` as a folder.
3. Review the changes and commit them to `main` with a message such as `Add trilingual Mer Tun website`.
4. Open **Settings → Pages**.
5. Choose **Deploy from a branch**, branch **main**, folder **/(root)**, then save.
6. Wait for the Pages deployment to complete and open the URL provided by GitHub.
7. Check all three languages, filters, images, mobile layout and a details dialog at the published URL.

Expected project URL: https://viktoria-voskanyan.github.io/armenia-homes/ (active only after Pages is enabled and deployment completes).

## Demo content

All listings, prices, floor areas and property descriptions are fictional sample data. Images are AI-generated concepts, not photographs of listed properties. This is a static portfolio demo, not a live real estate marketplace. It does not submit enquiries or process transactions. There are 66 fictional listings: six for each of Armenia’s ten regions and six for Yerevan, including three sale and three rental examples in each. This is not a comprehensive real-world inventory of Armenia.

Google Fonts are an optional online dependency. The local system-font fallback supports offline use. All site images are bundled locally. No API keys, backend, database or analytics are used.


## Property galleries

Each of the 66 listings has its own unique, region-inspired gallery: exterior, living room and bedroom. Previous/next arrows and photo selectors work on cards and in the details dialog. Left/right keyboard arrows and horizontal touch swipes also work. Each property remembers its current photo while filtering or switching languages in the same page session. The galleries contain fictional concepts, not real property photographs.

The three views of each property are stored efficiently in a single local WebP strip, with CSS showing one square view at a time. No gallery asset is shared by two different listings. Original generated artwork is retained in the working project; the download includes compressed WebP versions for faster loading.


## Currency conversion

The header currency selector switches between AMD, USD and EUR. Prices and the maximum-price input use the selected currency, while original listing prices and active budget filters remain stored in AMD. Changing currencies preserves the current filter meaning; displayed conversions are rounded and marked approximate. The selected currency is remembered on this device.

Fixed reference rates published by the Central Bank of Armenia for **22 October 2026**: 1 USD = 361.33 AMD and 1 EUR = 405.23 AMD. Source: https://www.cba.am/en/exchange-rates-archive . These are a dated snapshot, not live bank buy/sell rates. The date and source are shown in the interface when foreign currency is selected. Update the constants in script.js and the audit record in exchange-rates.json together when refreshing rates.

## Region inventory

Choose All to see all six offers in a region together, or Buy / Rent for three offers of each type. Existing listing IDs, galleries and saved selections are preserved. Every listing has a unique gallery with three different views. Extra cities and listings are defined inline in script.js so the page also works when opened directly from a local file. extra-properties.json is the readable source-data record for the added listings.

## Agency navigation
The header opens separate agency, home-guide, saved-home and contact dialogs. Saved homes persist on this device. Each listing includes an enquiry draft action and a unique AH reference. The contact form displays a local draft only: no message is sent. Phone and email are intentionally awaiting real agency details.

Brand: Մեր Տուն — Mer Tun. Tagline: Այստեղ քեզ զգա ինչպես քո տանը։
