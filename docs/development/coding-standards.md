# FLVRTX Coding Standards

This document defines the coding standards for all development within the FLVRTX ecosystem.

---

# General Principles

- Write readable code before clever code.
- Prefer reusable components over duplicated markup.
- Keep functions small and focused.
- Follow a component-first architecture.
- Every change should improve maintainability.

---

# Blade Templates

## File Naming

Use lowercase with hyphens.

Examples:

recipe/hero.blade.php
learn/card.blade.php
watch/video.blade.php

---

## Components

Reusable UI belongs in:

resources/views/components/ui/

Examples:

- button
- badge
- card
- section
- section-header

Website-wide reusable components belong in:

resources/views/components/global/

Examples:

- author-card
- share
- reading-progress
- back-to-top

---

## Blade Formatting

- Use 4-space indentation.
- Keep one Blade directive per line.
- Avoid deeply nested conditions.
- Extract repeated markup into components.

Preferred:

@if(has_post_thumbnail())

    ...

@endif

---

# Tailwind CSS

## Utility Classes

Prefer Tailwind utilities over custom CSS.

Avoid inline styles.

---

## Component Styling

Use design tokens.

Examples:

bg-primary
text-text
border-border

Do not hardcode colors.

---

## Layout

Use:

<x-ui.section>

<x-ui.container>

for page layouts.

---

# JavaScript

Use ES Modules.

Keep app.js minimal.

Business logic belongs in:

resources/js/modules/

Examples:

- alpine.js
- lucide.js
- navigation.js
- reading-progress.js

---

# PHP

- Follow WordPress Coding Standards.
- Follow PSR-12 where applicable.
- Avoid global functions when helpers exist.
- Keep business logic outside Blade templates.

---

# ACF

Every custom field must:

- Have a meaningful field name.
- Use snake_case.
- Group related fields together.

Example:

prep_time
cook_time
difficulty

---

# Performance

- Lazy load images.
- Optimize assets before production.
- Keep JavaScript modular.
- Avoid unnecessary plugins.

---

# Accessibility

Every page should include:

- Semantic headings
- Alt text
- Keyboard accessibility
- Visible focus states
- Sufficient color contrast

---

# Git

Commit messages should be descriptive.

Examples:

feat: add recipe hero component

fix: improve mobile navigation

docs: add architecture guide

refactor: modularize JavaScript

---

# Documentation

Every major architectural decision should be documented in FLVRTX OS before implementation.
