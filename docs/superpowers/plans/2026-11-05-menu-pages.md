# Menu Pages Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Build the MENU landing page and separate drink, sweets, and food pages for Jobicafe.

**Architecture:** Keep the site as static HTML and shared plain CSS. Each page will use the same warm café visual language, navigation, and responsive product-card styles. Existing drink images will be used; sweets and food image areas will show intentional photo placeholders until their separately generated assets are available.

**Tech Stack:** HTML5, CSS3, Google Fonts (Playfair Display).

**Spec:** `docs/superpowers/specs/2026-10-29-menu-design.md`

## Global Constraints

- Use plain HTML and CSS; do not add Bootstrap or JavaScript.
- Use warm colors and Playfair Display for headings.
- Keep category pages separate: drinks, sweets, and food.
- Use sample menu copy and pricing where actual menu details are unavailable.
- Avoid broken image references; use available local drink images and clear placeholders for missing sweets/food photos.

## Review Focus

- Small screens: layouts should collapse to one column without horizontal scrolling.
- Missing sweets/food image assets: placeholders should remain intentional and readable.
- Long Japanese product names and descriptions: card content should wrap without clipping.
- Keyboard navigation: every category and return link should be a native anchor.
- Local drink image paths: use files already present under `images/menu/`.

---

### Task 1: MENU landing page and shared styles

**Files:**
- Modify: `menu.html`
- Modify: `menu-style.css`

**Interfaces:**
- Produces shared page layout, navigation, category tiles, and product-card styles for the three detail pages.

- [ ] Build the MENU landing page with the café heading, short introduction, and links to drink, sweets, and food pages.
- [ ] Add the shared warm palette, Playfair Display heading style, responsive layout, focus-visible link treatment, and reusable card styles.
- [ ] Review HTML and linked local paths, then commit this completed page checkpoint.

### Task 2: Drink page

**Files:**
- Create: `menu-drink.html`

**Interfaces:**
- Consumes shared layout and product-card styles from `menu-style.css`.
- Uses existing files in `images/menu/` for drink products.

- [ ] Add the drink page title, category navigation, and sample drink cards with local images, names, descriptions, and prices.
- [ ] Review HTML and image paths, then commit this completed page checkpoint.

### Task 3: Sweets page

**Files:**
- Create: `menu-sweets.html`

**Interfaces:**
- Consumes shared layout and product-card styles from `menu-style.css`.
- Uses intentional photo placeholders until sweets images are available.

- [ ] Add the sweets page title, category navigation, and sample sweets cards with names, descriptions, and prices.
- [ ] Review HTML, then commit this completed page checkpoint.

### Task 4: Food page

**Files:**
- Create: `menu-food.html`

**Interfaces:**
- Consumes shared layout and product-card styles from `menu-style.css`.
- Uses intentional photo placeholders until food images are available.

- [ ] Add the food page title, category navigation, and sample food cards with names, descriptions, and prices.
- [ ] Review HTML, then commit this completed page checkpoint.
