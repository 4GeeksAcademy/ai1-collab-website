# Style Guide

## Company Details
- Name: Petco Animal Supplies, Inc.
- Slogan: Your Neighborhood Pet Hub
- Primary Logo (homepage): `Images/NEW Petco Logo 2025.png`

## Design System Source
This guide reflects the current implementation in `index.html`.

## Color System

### Core Brand Colors
- Brand Navy: `#00205B` (primary CTAs, headings, key surfaces)
- Brand Blue: `#123E8A` (hover/secondary emphasis)
- Brand Soft: `#E8EEF8` (input backgrounds, subtle highlights)
- Surface: `#F7FAFF` (page background base)
- White: `#FFFFFF` (cards, sections, high-contrast buttons)

### Supporting Usage
- Borders: use low-contrast navy transparency (example: `border-brand/10`)
- Text hierarchy:
    - Primary: `brand`
    - Secondary: `brand/80` to `brand/90`
    - Inverse on dark backgrounds: `white`, `white/85`, `white/90`
- Rating stars/accent: amber tone (`text-amber-500`)

## Typography
- Primary font family: `"DM Sans", sans-serif`
- Source: Google Fonts (`DM Sans` weights 400, 500, 700, 800)
- Font usage:
    - Hero and section titles: extra-bold (`font-extrabold`)
    - Product and card titles: bold (`font-bold`)
    - Buttons and controls: semibold to bold (`font-semibold` / `font-bold`)
    - Body copy: regular to medium

## Layout and Spacing
- Content max width: `max-w-7xl`
- Primary horizontal spacing:
    - Mobile: `px-4`
    - Small: `sm:px-6`
    - Large: `lg:px-8`
- Section rhythm: generally `py-12`
- Header behavior: sticky header with blur and subtle border

## Shape Language
- Primary radius: `rounded-3xl` (cards, feature blocks, media)
- Interactive controls: `rounded-full` (buttons, search bar, icon buttons)
- Secondary radius: `rounded-2xl` (inner media elements)

## Shadows and Depth
- Custom elevation token:
    - `soft`: `0 20px 45px rgba(0, 32, 91, 0.12)`
- Usage: key cards, hero containers, dropdown menus, and media blocks

## Motion and Effects
- Initial page transition:
    - White overlay fade-out (`fade-screen`, 1s)
    - Content fade-in (`fade-content`, 0.85s, slight delay)
- Hover interactions:
    - Cards lift subtly (`hover:-translate-y-1`)
    - Category/product images scale on hover (`group-hover:scale-105`)
    - Buttons shift to stronger contrast on hover
- Accessibility:
    - Reduced motion support is implemented via `prefers-reduced-motion: reduce`

## Components and Interaction Patterns
- Header includes:
    - Brand logo
    - Search input with filled pill container
    - Pill navigation controls
    - Account avatar trigger with hover/focus dropdown
- Product/category cards:
    - Media-first layout
    - Bold title + prominent price
    - Full-width primary CTA for add-to-cart actions
- Footer patterns:
    - Pill action buttons
    - Hover/focus reveal help menu
    - Outlined social icon buttons with inverse hover state

## Implementation Notes
- Tailwind CSS is loaded via CDN and extended in-page with custom `colors` and `boxShadow` tokens.
- The style guide should be updated whenever `tailwind.config` tokens in `index.html` are changed.

