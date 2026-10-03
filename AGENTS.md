# BestLink Website

## Architecture

Astro static site. Content/code separation:
- `src/data/products.json` — all product data (model, specs, images, category)
- `src/pages/` — Astro pages (index, products, about, contact)
- `src/components/` — reusable Astro components (Header, Footer, ProductCard)
- `src/layouts/` — page layouts (Base)
- `public/images/products/` — product images

## Development

```bash
npm run dev       # Start dev server
npm run build     # Build for production
npm run preview   # Preview production build
```

## Adding Products

Edit `src/data/products.json` — add an entry to the `products` array. Pages auto-generate.

## Deployment

GitHub Actions (`.github/workflows/deploy.yml`) pushes to SiteGround on push to `main`.
Four secrets required (set in GitHub repo Settings → Secrets → Actions):
- `SFTP_HOST`     — FTP host address
- `SFTP_PORT`     — FTP port (default 21)
- `SFTP_USER`     — FTP username
- `SFTP_PASSWORD` — FTP password

## Full Astro docs: https://docs.astro.build

Consult these guides before working on related tasks:
- [Adding pages, dynamic routes, or middleware](https://docs.astro.build/en/guides/routing/)
- [Working with Astro components](https://docs.astro.build/en/basics/astro-components/)
- [Adding styles or using Tailwind](https://docs.astro.build/en/guides/styling/)
