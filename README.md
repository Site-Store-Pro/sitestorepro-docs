# Site Store Pro Documentation

Official developer documentation for **Site Store Pro**, a Laravel-based e-commerce, CMS, and helpdesk platform.

Live site: [docs.sitestorepro.com](https://docs.sitestorepro.com)

## About Site Store Pro

Site Store Pro combines a high-performance e-commerce storefront, a flexible CMS site-builder, and a complete customer support system. Built on Laravel 13, Livewire 3, Tailwind CSS, and Alpine.js, it provides everything needed to run an online store: product catalog management, multi-gateway payments, CMS pages, and helpdesk ticketing.

## Documentation structure

The docs are organized into two tabs:

### Documentation

- **Getting Started** — Introduction, installation, user roles, demo store
- **Storefront** — Shop catalog, product details, cart & checkout, digital downloads
- **Admin: Products** — Products overview, variants & pricing, inventory & warehouse, bulk import, product duplication, product reviews
- **Admin: Orders & Sales** — Orders & refunds, discounts engine, shipping & tax, email notifications
- **Admin: CMS** — Pages & posts, downloads manager, code embeds, form builder, list menus & shortcodes, header/footer builder, navigation builder
- **Payments & Subscriptions** — Overview, Stripe, Paddle, PayPal, subscriptions, webhooks
- **Plugins & Extensions** — Plugin system, display plugins, shipping plugins, custom plugins
- **Support & Helpdesk** — Ticketing, knowledge base
- **Configuration** — Global settings, currency & VAT, multilingual, security, production checklist

### API & Webhooks

- **Routes Reference** — Storefront routes, admin routes, webhook endpoints
- **Shortcode Reference** — Shortcode reference, shortcode pipelines

## Local development

This documentation is built with [Mintlify](https://mintlify.com). Install the CLI to preview changes locally:

```bash
npm i -g mint
```

Run the dev server from the repo root (where `docs.json` lives):

```bash
mint dev
```

Preview at `http://localhost:3000`.

## Publishing

Changes pushed to the default branch of this repo are deployed automatically to [docs.sitestorepro.com](https://docs.sitestorepro.com) via the Mintlify GitHub app.

## Repository layout

```text
.
├── docs.json              # Site config, theme, and navigation
├── introduction.mdx       # Landing page
├── installation.mdx
├── user-roles.mdx
├── demo-store.mdx
├── storefront/            # Storefront pages
├── admin/                 # Admin panel docs (products, orders, etc.)
├── cms/                   # CMS builder docs
├── payments/              # Payment gateways & subscriptions
├── plugins/               # Plugin system & extensions
├── helpdesk/              # Support & ticketing
├── configuration/         # Global config & production checklist
├── api/                   # Routes, webhooks, shortcode reference
├── logo/                  # Brand assets
└── favicon.svg
```

## Contributing

1. Create a branch from `main`.
2. Edit or add `.mdx` files. Update `docs.json` if you add pages or change navigation.
3. Preview with `mint dev`.
4. Open a pull request.

## Troubleshooting

- Dev server not running: run `mint update` to get the latest CLI.
- Page loads as 404: confirm you're running `mint dev` from the folder containing `docs.json`.

## Resources

- [Site Store Pro website](https://sitestorepro.com)
- [Mintlify documentation](https://mintlify.com/docs)
- [Mintlify components](https://mintlify.com/docs/components)