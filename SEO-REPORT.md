# BT Tiles (Bharathiya Tiles) — On-Page SEO Report

Site: https://bttiles.com/ · Date: 2026-10-06 · Scope: on-page SEO only (no design, layout, image or section changes)

All changes were verified in headless Chrome at desktop (1366px) and mobile (390px) widths by comparing the computed style of every visible element before and after. Apart from the intended text edits, rendering is identical.

---

## A. Audit (before changes)

| Page URL | Title | Meta desc | H1 count / text | Heading order | Words | Missing/weak alts | Dupes | Canonical | Schema | Other issues |
|---|---|---|---|---|---|---|---|---|---|---|
| / (index.html) | Home - Bharathiya Tiles (+ 2nd `<title>`) | none | **3**: "Bharathiya Tiles", "WE WILL PROVIDE YOUTHE BEST SERVICE", Tamil tagline | H2 logo → H1 → H3 → H1 → H2… | 905 | 23 | — | none | none | 2 full HTML documents concatenated; keyword-stuffed caps line; typos ("YOUTHE", "We'r Prodviding"); "Get started" → 404 page |
| /all-tiles.html | All Tiles - Bharathiya Tiles | none | **0** | H2 → H4 → H3 | 350 | 25 | — | none | none | duplicate viewport |
| /paints.html | Paints - Bharathiya Tiles | none | **2** | H1 → H2 → H3 → H1 | 661 | 15 | — | none | none | — |
| /sanitary.html | Sanitarywares - Bharathiya Tiles | none | **0** | H2 → H5 → H3 → H4 | 2019 | 17 | — | none | none | 2 documents concatenated |
| /watertank.html | Water Tank - Bharathiya Tiles | none | **0** | H2 → H5 → H3 | 436 | 15 | — | none | none | **3** documents / 3 titles ("Premium Sanitaryware", "Premium Sinks") |
| /fiting.html | CP Fittings - Bharathiya Tiles | none | 1: "our doors" (wrong) | H2 → H5 → H3 → H1 | 269 | 15 | — | none | none | faucets labelled "wooden Door", alt "Premium Door" |
| /sink.html | Kitchen Sinks - Bharathiya Tiles | none | **0** | H2 → H5 → H3 | 456 | 15 | — | none | none | — |
| /bathtub.html | Bath Tub - Bharathiya Tiles | none | 1: "Our Projects" | H2 → H5 → H3 → H1 | 303 | 15 | — | none | none | 2 documents |
| /chimmey.html | Chimney & Hobs - Bharathiya Tiles | none | 1: "Our products" | H2 → H5 → H3 → H1 | 315 | 15 | — | none | none | 2 documents |
| /door.html | Doors - Bharathiya Tiles | none | 1: "OUR DOORS" | H2 → H5 → H3 → H1 | 278 | 15 | — | none | none | 2 documents |
| /manhole.html | Manhole Covers - Bharathiya Tiles | none | 1: "Premium Manhole Covers" | H2 → H5 → H3 → H1 | 303 | 21 | — | none | none | 2 documents |
| /tile-accessories.html | Tiles Accessories - Bharathiya Tiles | none | **0** | H2 → H4 | 112 | 19 | — | none | none | thin content |
| /waterproofing.html | Waterproofing - Bharathiya Tiles | none | **0** | H2 → H4 | 113 | 18 | — | none | none | 2 documents; thin |
| /elevation.html | Elevation Tiles - Bharathiya Tiles | none | 1: "Elevation Feature Tiles" | OK | 557 | 31 | — | none | none | — |
| /kitchen-wall-tiles.html | Kitchen Wall Tiles - Bharathiya Tiles | none | 1: "Kitchen Tiles" | OK | 151 | 13 | — | none | none | — |
| /livingroomtiles.html | Living Room Tiles - Bharathiya Tiles | none | 1: "Living Room Tiles" | OK | 269 | 17 | — | none | none | — |
| /rooftiles.html | Roof Tiles - Bharathiya Tiles | none | **0** | — | 107 | 13 | — | none | none | **no content at all** (nav + footer only) |
| /page-contact.html | Contact Us - Bharathiya Tiles | none | 1: "Contact Us" | OK | 171 | 15 | — | none | none | map embed searches "Bharathiya Tiles **Cuddalore**"; phone shown 3 different ways |
| /cladding-tiles.html, /floor-tiles.html | Page not found | none | 1 | — | 94 | 1 | **dup title** | none | none | soft-404 pages returning 200 |
| /tiles-pages/* (8 pages) | "Kitchen Tiles · …" ×5, "Tiles Navbar · animated" ×2 | none | 0–1 | — | 144–721 | ~15 each | **dup titles** | none | none | bathroom-wall/floor + kitchen-wall/floor/kitchentiles are byte-identical copies of the kitchen template |

**Site-wide:** `lang="en"` (not en-IN) · no Open Graph/Twitter tags · `robots.txt` → 404 · `sitemap.xml` → 404 · `https://www.bttiles.com/` serves a duplicate 200 (no redirect) · `/index.html` duplicates `/` · http → https already 301 ✔ · footer links to `about.html` and `contact.html` are 404 · footer "Tiles" → home, "Tiles Accessories" → all-tiles, "Sanitary Wares" → contact (wrong targets) · ~22 nav icons per page without alt; Waterproofing/Tile-accessories icons had alt "Bath Tub" · no `loading="lazy"` on most images · viewport on several pages had `user-scalable=0` (mobile accessibility flag) · HTTrack "Mirrored from…" comments left in source.

---

## B. Per-page changes (Element | Current | Optimized)

### Home — `/`
| Element | Current | Optimized |
|---|---|---|
| Title | Home - Bharathiya Tiles | Tile Dealer in Pondicherry \| Bharathiya Tiles (BT Tiles) |
| Meta description | — | Bharathiya Tiles is a trusted tile dealer in Pondicherry for wholesale tiles, paints, sanitaryware & water tanks, serving Cuddalore, Villupuram & OMR. Visit us. |
| H1 | 3 H1s | **One H1:** "TRUSTED TILE DEALER IN PONDICHERRY" (was "WE WILL PROVIDE YOUTHE BEST SERVICE") |
| Hero "Bharathiya Tiles" | `<h1>` | `<h2 class="hvs-title keep-h1-style">` (looks identical) |
| Tamil tagline | `<h1>` | `<div>` with the same class (looks identical) |
| Section H2 | Explore Modern Tiles Stone & Agency | Your Tile Showroom in Pondicherry |
| About paragraph | "…largest tiles shop… TILES WHOLESALERS / TILES SHOWROOM / TILES DEALERS IN PONDICHERRY" | "Bharathiya Tiles is a leading tile dealer in Pondicherry and the largest tile shop in Puducherry… As a tile wholesaler in Pondicherry, we supply wholesale tiles… visit our tile showroom in Pondicherry, where you will also find paints, sanitaryware and water tanks." (same length, no stuffing) |
| CTA button | "Get started" → page-about.html (404) | "Visit Our Showroom" → page-contact.html |
| Eyebrow | PONDICHERRY'S LARGEST SHOWROOM | PONDICHERRY'S LARGEST TILE SHOWROOM |
| "Why choose" intro | From flooring to fittings… | From tiles and paints to sanitaryware… |
| On-Time Delivery card (**service-area line**) | Careful handling and prompt delivery across Pondicherry, so your project timeline never slips. | Prompt delivery across Pondicherry, Cuddalore, Villupuram, Tindivanam, Chidambaram and OMR. |
| H2 | Discover Our Flooring Services & Quality at Bharathiya Tiles | Tiles, Paints & Sanitaryware Quality at Bharathiya Tiles |
| Paragraph | Your home reflects… largest tile retailer… | …we are a trusted paint dealer, sanitaryware dealer and water tank dealer in Pondicherry, so your floors, walls and bathroom fittings come from one place… |
| Service cards | Sanitary Ware / "Premium bathroom fixtures…" | Sanitaryware / "Premium sanitaryware and bathroom fittings…" |
| Banner H3 | We'r Prodviding Quality flooring Services | Your Trusted Tile Shop in Pondicherry |
| Banner button | Free Consultations | Free Tile Consultation |
| Schema | — | HomeGoodsStore + WebSite JSON-LD |

### Product and category pages
| Page | Title | H1 (old → new) | Copy change |
|---|---|---|---|
| all-tiles | Tile Shop in Pondicherry \| Wall & Floor Tiles \| BT Tiles | none → "TILE SHOP IN PONDICHERRY" (was H2 "OUR PRODUCTS"); sub-label "Our project" → "Our Tiles" | — |
| paints | Paint Dealer in Pondicherry \| Berger Paints \| BT Tiles | "Premium colour for every bharathiya home" → "**Paint Dealer** in Pondicherry"; 2nd H1 → H2 | "…powered by Bharathiya Tiles, Lawspet." → "…from your paint wholesaler in Pondicherry." |
| sanitary | Sanitaryware Dealer in Pondicherry \| Bharathiya Tiles | none → "Sanitaryware Dealer in Pondicherry" (hero H2 promoted) | "the leading sanitary ware store in Pondicherry" → "a leading sanitaryware dealer and tile dealer in Pondicherry" |
| watertank | Water Tank Dealer in Pondicherry \| Bharathiya Tiles | none → "Water Tank Dealer in Pondicherry" | "Water tanks store clean water…" → "As a water tank dealer in Pondicherry, we supply tanks that store clean water…" |
| fiting | CP Bathroom Fittings in Pondicherry \| Bharathiya Tiles | "our doors" → H2 "Our CP Fittings"; new H1 "CP Bathroom Fittings in Pondicherry" | product labels "wooden Door" → Chrome Basin Faucet / Gold Finish Wall Mixer / Overhead Shower / CP Bathroom Fitting (matching the photos) |
| sink | Kitchen Sinks in Pondicherry \| Steel Sinks \| BT Tiles | none → "Kitchen Sinks in Pondicherry" | "…a trusted tile dealer in Pondicherry, our kitchen sinks retain…" |
| bathtub | Bathtubs in Pondicherry \| Jacuzzi & Acrylic \| BT Tiles | "Our Projects" → H2 "Our Bathtub Projects"; H1 "Luxury Bathtubs in Pondicherry" | "…a sanitaryware dealer in Pondicherry, we offer premium bathtubs…" |
| chimmey | Kitchen Chimney & Hobs in Pondicherry \| Bharathiya Tiles | "Our products" → H2 "Our Chimney Products"; H1 "Chimney & Hobs in Pondicherry" | "At Bharathiya Tiles in Pondicherry…" |
| door | PVC & Wooden Doors in Pondicherry \| Bharathiya Tiles | "OUR DOORS" → H2; H1 "PVC & Wooden Doors in Pondicherry" | "At Bharathiya Tiles in Pondicherry…" |
| manhole | Manhole Covers in Pondicherry \| FRP Covers \| BT Tiles | "Premium Manhole Covers" → H2; H1 "Manhole Covers in Pondicherry" | "At Bharathiya Tiles in Pondicherry…" |
| tile-accessories | Tile Adhesive, Grout & Spacers in Pondicherry \| BT Tiles | none → "Tile Accessories in Pondicherry" | — |
| waterproofing | Waterproofing Products in Pondicherry \| Bharathiya Tiles | none → "WATERPROOFING IN PONDICHERRY"; "Our project" → "Our Products" | — |
| elevation | Elevation Tiles in Pondicherry \| Bharathiya Tiles | unchanged (styled 3-line H1) | "…our elevation tiles in Pondicherry transform every facade…" |
| kitchen-wall-tiles | Kitchen Wall Tiles in Pondicherry \| Bharathiya Tiles | unchanged | eyebrow "Bharathiya Tiles · Collection" → "Bharathiya Tiles · Pondicherry" |
| livingroomtiles | Living Room Tiles in Pondicherry \| Bharathiya Tiles | unchanged | "…collection at our Pondicherry tile showroom…" |
| rooftiles | Roof Tiles Dealer in Pondicherry \| Bharathiya Tiles | — (page has no content) | set to **noindex** until content is added |
| page-contact | Contact Bharathiya Tiles \| Tile Showroom in Pondicherry | "Contact Us" → "Contact Bharathiya Tiles" | H2 "Get in touch with us" → "Visit our tile showroom"; text → "Call our tile dealer in Pondicherry for tile, paint, sanitaryware and water tank prices."; phone shown as +91-7500275005 |

Each page also has a unique meta description (140–160 chars). You can read them in each file's `<head>`.

---

## C. Ready-to-paste code (already applied in the files)

**Head block (home example)**
```html
<html lang="en-IN">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Tile Dealer in Pondicherry | Bharathiya Tiles (BT Tiles)</title>
<meta name="description" content="Bharathiya Tiles is a trusted tile dealer in Pondicherry for wholesale tiles, paints, sanitaryware &amp; water tanks, serving Cuddalore, Villupuram &amp; OMR. Visit us.">
<meta name="robots" content="index, follow, max-image-preview:large">
<link rel="canonical" href="https://bttiles.com/">
<meta property="og:type" content="website">
<meta property="og:site_name" content="Bharathiya Tiles">
<meta property="og:locale" content="en_IN">
<meta property="og:title" content="Tile Dealer in Pondicherry | Bharathiya Tiles (BT Tiles)">
<meta property="og:description" content="…same as meta description…">
<meta property="og:url" content="https://bttiles.com/">
<meta property="og:image" content="https://bttiles.com/images/tiles/about-img.png">
<meta name="twitter:card" content="summary_large_image">
```

**Schema JSON-LD** (on `/` and `/page-contact.html`; validated as JSON)
```json
{
  "@context": "https://schema.org",
  "@graph": [{
    "@type": "HomeGoodsStore",
    "@id": "https://bttiles.com/#business",
    "name": "Bharathiya Tiles",
    "alternateName": "BT Tiles",
    "url": "https://bttiles.com/",
    "logo": "https://bttiles.com/images/bt_logo.png",
    "image": "https://bttiles.com/images/tiles/about-img.png",
    "telephone": "+91-7500275005",
    "email": "support@bttiles.com",
    "address": {
      "@type": "PostalAddress",
      "streetAddress": "146/5, East Coast Road, opp. Raja Rajeshwari Kalyana Mandapam, Pakkamudayanpet, Kottupalayam",
      "addressLocality": "Puducherry", "addressRegion": "Puducherry",
      "postalCode": "605008", "addressCountry": "IN"
    },
    "hasMap": "https://www.google.com/maps/place/?q=place_id:ChIJtdsRP2xhUzoRtN110uGST5E",
    "openingHoursSpecification": [
      { "@type": "OpeningHoursSpecification", "dayOfWeek": ["Monday","Tuesday","Wednesday","Thursday","Friday","Saturday"], "opens": "09:45", "closes": "20:00" },
      { "@type": "OpeningHoursSpecification", "dayOfWeek": "Sunday", "opens": "09:45", "closes": "14:00" }
    ],
    "areaServed": ["Pondicherry","Cuddalore","Villupuram","Tindivanam","Chidambaram","OMR (Old Mahabalipuram Road)"],
    "hasOfferCatalog": { "@type": "OfferCatalog", "name": "Tiles, paints, sanitaryware and water tanks", "itemListElement": ["Tiles","Paints","Sanitaryware","Water Tanks","CP Bathroom Fittings","Kitchen Sinks"] },
    "sameAs": ["facebook", "instagram", "justdial", "indiamart profile URLs"]
  }]
}
```
(The live file uses typed `City` / `OfferCatalog` objects and full sameAs URLs. This listing is shortened.)

`geo` and `priceRange` are **intentionally left out** until the owner confirms them (see E).

**Alt-text examples (applied by image path)**
- `images/tiles/about-img.png` → "Bharathiya Tiles showroom storefront, tile dealer in Pondicherry"
- `images/resource/about-two.png` → "Hexagon mosaic bathroom wall tiles with wash basin from Bharathiya Tiles"
- `images/tiles/elevation/elevation (N).jpg` → "Exterior elevation tiles on a house facade, Bharathiya Tiles Pondicherry"
- `images/tank.webp` → "Water storage tank from Bharathiya Tiles, water tank dealer in Pondicherry"
- nav icons → their category name (Home, Tiles, Paints, Sanitaryware, CP Fittings…)

**Suggested descriptive file names** (renaming is optional and needs every `src` updated, so it was not done):
`about-img.png` → `bharathiya-tiles-showroom-pondicherry.png` · `about-two.png` → `hexagon-mosaic-bathroom-wall-tiles.png` · `elevation (1).jpg` → `elevation-tiles-pondicherry-1.jpg` · `tank.webp` → `water-tank-dealer-pondicherry.webp` · `OIP.webp` → `berger-paints-pondicherry.webp` · `FLOR.avif` → `bathroom-floor-tiles.avif` · `frp1.jpg` → `frp-manhole-cover-1.jpg`

**robots.txt**
```
User-agent: *
Allow: /
Disallow: /fonts/*.html
Disallow: /images/resource/*.html
Sitemap: https://bttiles.com/sitemap.xml
```

**.htaccess** — www → non-www and `/index.html` → `/` 301 redirects, gzip and browser caching. http → https is already handled by the host.

**sitemap.xml** — 17 indexable URLs.

---

## D. Checklist of changes

- [x] Unique title (45–60 chars) on all 28 pages; primary or page keyword first, brand last
- [x] Unique meta description (140–160 chars) on all 18 public pages
- [x] Exactly one H1 on every indexable page; home H1 contains "Tile Dealer in Pondicherry"
- [x] Demoted stray H1s keep their original size via `.keep-h1-style` (css/style.css)
- [x] `.sec-title-two h1` added next to `.sec-title-two h2` selectors so promoted H1s look identical (css/style.css, css/responsive-fixes.css)
- [x] Rewrote existing copy at about the same length; primary keyword in the first 100 words of home; secondary keywords spread once each
- [x] Service-area towns placed once each in existing home copy (On-Time Delivery card), in the meta descriptions and in schema
- [x] Typos fixed in rewritten text ("YOUTHE", "We'r Prodviding", "CPI Fittings")
- [x] Alt text on every content image; wrong alts fixed ("Bath Tub" on waterproofing icon, "Premium Door" on faucets, "Justdial" on IndiaMART)
- [x] `loading="lazy"` on below-the-fold images (header, category nav and floating icons kept eager)
- [x] Footer links fixed: Tiles → all-tiles, Tile Accessories → tile-accessories, Sanitaryware → sanitary, Contact → page-contact
- [x] Phone shown as +91-7500275005 and linked `tel:+917500275005` in header, footer, about section and contact page
- [x] WhatsApp link already existed; left unchanged
- [x] Duplicate `<!DOCTYPE>/<html>/<head>/<body>/<title>/viewport` tags removed (DOM-neutral)
- [x] `lang="en-IN"`, single clean viewport (pinch-zoom no longer blocked)
- [x] Canonical, Open Graph and Twitter tags on indexable pages
- [x] LocalBusiness (HomeGoodsStore) + WebSite JSON-LD; no FAQPage schema
- [x] noindex on soft-404s, the duplicate `tiles-pages/*` templates and the empty roof-tiles page
- [x] robots.txt, sitemap.xml, .htaccess created
- [x] HTTrack mirror comments removed

---

## E. [NEEDS INPUT FROM OWNER]

1. **Geo coordinates** (latitude/longitude of the showroom) — add `"geo": {"@type":"GeoCoordinates","latitude":…, "longitude":…}` to the schema.
2. **priceRange** — e.g. "₹₹" — add to the schema.
3. **Contact-page map** — the embed searches "Bharathiya Tiles **Cuddalore**". Is there a Cuddalore branch, or should it point to the ECR / Kottupalayam showroom?
4. **Business name for NAP** — Google Business Profile name: "Bharathiya Tiles" or "BT Tiles"? Schema uses Bharathiya Tiles with BT Tiles as alternate name.
5. **Address in footer** — the footer has no address, and adding visible text was out of scope. Approve adding it for full NAP consistency?
6. **About page** — footer "About" links to `about.html`, which doesn't exist (404). Create the page, or point the link elsewhere?
7. **Roof tiles page** — has no content and is noindexed until real content is added.
8. **tiles-pages/** — the bathroom wall/floor and kitchen wall/floor pages are identical kitchen templates, linked from Tile Accessories ("Tiles Adhesive" → bathroom-wall.html). Real content or corrected links are needed.
9. **Service-area line** — the brief said it was already on the site; it wasn't in the code. Its wording was placed into the existing delivery card instead. Confirm you deliver to all six areas.
10. **Brands stocked** (beyond Berger, Habito, Acura seen on the storefront) — useful for future copy and schema `brand` fields.
11. **Social links** — LinkedIn and YouTube icons in the footer link to `#`. Provide URLs or remove them.
