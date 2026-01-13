---
name: kiki-brand-style-guide
description: KIKI The Brand style guide - colors, typography, and design system rules
---

# KIKI Brand Style Guide

**ALWAYS follow this style guide when working on KIKI The Brand Shopify theme.**

## Color Palette

The following brand colors MUST be used throughout the theme:

| Color Name    | Hex Code  | Usage                                                     |
| ------------- | --------- | --------------------------------------------------------- |
| **Mahogany**  | `#4a0000` | Primary buttons, large image backgrounds, accent elements |
| **Baby Pink** | `#f6c3c8` | Announcements, borders, secondary accents                 |
| **Creme**     | `#f8f6f1` | Body background, header, footer, drawer background        |
| **White**     | `#ffffff` | Small image backgrounds, button text                      |
| **Black**     | `#000000` | Text, footer text                                         |

### CSS Color Variables

Always use these CSS variables when referencing colors:

- `--color-mahogany: #4a0000`
- `--color-baby-pink: #f6c3c8`
- `--color-creme: #f8f6f1`
- `--color-white: #ffffff`
- `--color-black: #000000`

### Utility Classes Available

- Text colors: `.text-mahogany`, `.text-baby-pink`, `.text-creme`, `.text-white`, `.text-black`
- Background colors: `.bg-mahogany`, `.bg-baby-pink`, `.bg-creme`, `.bg-white`, `.bg-black`

## Typography System

### H2 - Large Headers

- **Font:** PP Neue Corp Extended Medium (fallback: theme default)
- **Size:** 24px
- **Weight:** 500
- **Line Height:** 100% (1)
- **Letter Spacing:** 2% (0.02em)
- **CSS Variables:** `--font-h2-family`, `--font-h2-size: 24px`, `--font-h2-weight: 500`, `--font-h2-line-height: 1`, `--font-h2-letter-spacing: 0.02em`

### H3 - Medium Headers

- **Font:** PP Neue Corp Extended Medium (fallback: theme default)
- **Size:** 18px
- **Weight:** 500
- **Line Height:** 100% (1)
- **Letter Spacing:** 2% (0.02em)
- **CSS Variables:** `--font-h3-family`, `--font-h3-size: 18px`, `--font-h3-weight: 500`, `--font-h3-line-height: 1`, `--font-h3-letter-spacing: 0.02em`

### H4 - Body Headers

- **Font:** Work Sans Regular
- **Size:** 14px
- **Weight:** 400
- **Line Height:** 100% (1)
- **Letter Spacing:** 0
- **CSS Variables:** `--font-h4-family`, `--font-h4-size: 14px`, `--font-h4-weight: 400`, `--font-h4-line-height: 1`, `--font-h4-letter-spacing: 0`

### H5 - Small Caps

- **Font:** PP Neue Corp Wide Medium (fallback: theme default)
- **Size:** 10px
- **Weight:** 500
- **Line Height:** 100% (1)
- **Letter Spacing:** 1% (0.01em)
- **Transform:** UPPERCASE
- **CSS Variables:** `--font-h5-family`, `--font-h5-size: 10px`, `--font-h5-weight: 500`, `--font-h5-line-height: 1`, `--font-h5-letter-spacing: 0.01em`

## Implementation Rules

1. **Always use CSS variables** defined in `snippets/css-variables.liquid` for colors and typography
2. **Use utility classes** when possible (`.text-mahogany`, `.bg-baby-pink`, etc.)
3. **Maintain typography hierarchy** - use H2-H5 styles as defined above
4. **Work Sans** is loaded from Google Fonts and available for H4 headings
5. **PP Neue Corp** fonts require font files - use fallbacks until fonts are uploaded

## Key Files

- **Color & Typography Variables:** `snippets/css-variables.liquid`
- **Font Declarations:** `snippets/font-face.liquid`
- **Main Stylesheet:** `assets/theme.css.liquid`
- **Theme Settings:** `config/settings_data.json`

## Reference

- **Figma Design:** [KIKI WEBSITE - Copy](https://www.figma.com/design/W3HGF2W4ubKvxcH6nAZYhv/KIKI-WEBSITE--Copy-?node-id=1-2&m=dev)
- **Full Documentation:** `KIKI_STYLE_GUIDE_IMPLEMENTATION.md`
