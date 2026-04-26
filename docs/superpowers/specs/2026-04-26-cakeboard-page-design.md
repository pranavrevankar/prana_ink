# Cakeboard project page — Design

## Goal

Add a Cakeboard project entry to the personal site that opens an internal blog-style page with a cover image, intro, and three feature sections.

## Context

- Static HTML site. `index.html` lists projects/posts as `<article>` cards. Internal blog pages follow the layout in `blog-2025-09-01.html` (Tailwind via CDN, max-w-3xl, "Back to Home" nav).
- Images already in place: `assets/cover.jpg`, `assets/feature-1.jpg`, `assets/feature-2.jpg`, `assets/feature-3.jpg`.

## Changes

### 1. `index.html` — new article card

- Insert a new `<article>` immediately before the "Get in Touch" article (i.e., last project in the list).
- Tag: `Project` only. `data-tags="project"`.
- Title: **Cakeboard**
- Description (one line): A college project from 2013-2014 — an innovative way to keep all the components needed for breadboarding right with the breadboard itself.
- Link: `cakeboard.html` (internal, no `target="_blank"`).

### 2. `cakeboard.html` — new internal page

Mirror the structure and styling of `blog-2025-09-01.html`. Sections in order:

1. **Head** — same Tailwind config, favicon, title `Cakeboard - Pranav Revankar`, meta description.
2. **Nav** — `← Back to Home` link to `index.html`.
3. **Header**
   - `<h1>` "Cakeboard"
   - Meta line: `College project · 2013-2014` plus a `Project` tag pill (yellow).
4. **Cover image** — `assets/cover.jpg`, full width, rounded corners, alt text "Cakeboard prototype".
5. **Intro** — 2–3 short paragraphs explaining what Cakeboard is: breadboarding always meant scrambling to find resistors, LEDs, jumper wires; built a layered "cake" board that stores components in place — hence the name. Built during college, 2013-2014.
6. **Three feature sections**, each with a small `<h2>` heading, an image, and a one-line description:
   - **Feature 1 — Components, always at hand.** `assets/feature-1.jpg`. Store all the components you need for breadboarding right there, no more forgetting.
   - **Feature 2 — Built-in fuse switch.** `assets/feature-2.jpg`. Switch directly with a built-in fuse to prevent breadboard burn.
   - **Feature 3 — Wire cutter clip.** `assets/feature-3.jpg`. Also clip the wire cutter right below the Cakeboard.
7. **Footer** — same `© 2024 Pranav Revankar` style.

## Out of scope

- No new tag colors. No filter changes on `index.html`.
- No JS / interactivity beyond what `blog-2025-09-01.html` already has.
- No image optimization or resizing — use the JPGs as provided.
