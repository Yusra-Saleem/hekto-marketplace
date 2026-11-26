# Hekto Lifestyle Marketplace

> Production-grade multi-category furniture and home decor e-commerce platform built on Next.js 15, Sanity CMS, and Tailwind CSS.

## 1. System Overview

Hekto is an enterprise e-commerce web platform architected for modern lifestyle furnishings and interior decor. It integrates headless content management via Sanity Studio, client-side dynamic search filtering, an optimized checkout pipeline, and a pixel-perfect component design system.

The application leverages Next.js App Router for server-side rendering, sub-second route transitions, and responsive cross-device performance.

## 2. Technical Architecture

```
[ Client Browser ]
        │
        ▼
[ Next.js 15 Edge / App Router ] ── (Server Components & SSR)
        │
        ├──▶ [ Sanity CMS (Headless API) ] ── (Product Data & Inventory)
        ├──▶ [ Middleware Auth & Routing ] ── (Route Protection & Sessions)
        └──▶ [ Client State (Cart/Wishlist) ] ── (Persistent Storage)
```

### Technology Stack
- **Framework:** Next.js 15 (React 19, TypeScript)
- **Content Engine:** Sanity Headless CMS (`sanity.config.ts`, `sanity.cli.ts`)
- **Styling:** Tailwind CSS, PostCSS, Radix UI primitives
- **Icons & Assets:** Lucide React
- **Architecture:** Next.js Middleware, Server Actions, Dynamic Data Fetching

## 3. Core Functional Capabilities

- **Headless Catalog Management:** Real-time synchronization with Sanity CMS for product listings, variant attributes, inventory status, and promotional banners.
- **Advanced Product Filtering:** Instant client-side faceted search by category, price range, color palette, and customer ratings.
- **Stateful Shopping Cart:** Persistent shopping cart state supporting quantity mutations, coupon code applications, and live price recalculations.
- **Responsive Design System:** Fully accessible atomic UI components conforming to modern accessibility standards across mobile, tablet, and ultra-wide viewports.

## 4. Directory Structure

```
hekto-marketplace/
├── sanity.config.ts          # Sanity Studio CMS workspace configuration
├── sanity.cli.ts             # Sanity CLI deployment settings
├── middleware.ts             # Route protection and header manipulation
├── src/
│   ├── app/                  # App Router pages and API routes
│   ├── components/           # Reusable UI component library
│   ├── lib/                  # Sanity client and utility helpers
│   └── types/                # TypeScript interface definitions
├── public/                   # Static imagery and brand assets
├── tailwind.config.ts        # Design tokens and theme configuration
└── package.json              # Project dependencies and build scripts
```

## 5. Getting Started

```bash
git clone https://github.com/Yusra-Saleem/hekto-marketplace.git
cd hekto-marketplace

npm install
npm run dev
```

## 6. Author and License

- **Author:** Yusra Saleem
- **Portfolio:** [yusrasaleem.dev](https://yusrasaleem.dev)
- **License:** Licensed under the [MIT License](LICENSE).
<!-- timeline-sync -->
<!-- updated: 2026-11-26T14:06:42Z -->
