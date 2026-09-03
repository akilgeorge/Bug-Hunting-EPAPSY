# Reconnaissance

## Target

**Domain:** epapsy.gr

## Technology Observations

The target was observed using:

- WordPress
- Elementor / Elementor Pro
- WooCommerce-related functionality

## Publicly Accessible Areas Identified

- Homepage and informational pages
- Site search
- Volunteer form
- Newsletter form
- Complaint form
- `/my-account/`
- `/my-account/lost-password/`
- `/shop/`
- `/cart/`
- `/checkout/`
- Product page
- WordPress XML sitemaps
- Public author archives

## WordPress Sitemap

The main WordPress sitemap was accessible and exposed multiple
content categories including:

- Posts
- Pages
- Products
- Categories
- Tags
- Product categories
- Users

The posts sitemap contained a large number of public article URLs.
Individual article pages were not exhaustively tested because they
primarily contained informational content. Representative pages were
sampled to identify additional interactive functionality.

## Author Enumeration

The users sitemap exposed public author archive URLs. One publicly
accessible author archive was associated with the username:

`epapsy_admin`

This was documented as an informational/low-severity observation.

## WooCommerce Reconnaissance

The product sitemap contained one product URL.

The Shop, Cart, Checkout and Product pages displayed a store-preparation
placeholder during testing. No active purchasing or payment workflow was
available.

## Scope

Testing remained limited to the target domain and was performed using a
non-intrusive manual approach.
