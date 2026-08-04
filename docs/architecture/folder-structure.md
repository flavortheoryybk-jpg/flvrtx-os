# FLVRTX Theme Folder Structure

This document describes the directory structure of the FLVRTX WordPress theme built with Sage 11.

---

# Root Structure

```
app/
config/
public/
resources/
routes/
storage/
vendor/
```

---

# app/

Contains all PHP application logic.

```
app/
├── Helpers/
├── Providers/
└── View/
    └── Composers/
```

### Helpers

Reusable helper functions.

### Providers

Service providers responsible for bootstrapping the theme.

### View Composers

Inject reusable data into Blade templates.

Current composers:

- HomeComposer
- Navigation
- RecipeSchema

---

# resources/

Contains all frontend assets.

```
resources/

css/
fonts/
images/
js/
views/
```

---

## CSS

```
css/

base/
layout/
pages/
```

- base → Design tokens & typography
- layout → Shared layout utilities
- pages → Page-specific styles

---

## JavaScript

```
js/

app.js
editor.js

modules/
```

Modules include:

- alpine
- lucide
- navigation
- reading-progress
- back-to-top

---

## Views

```
views/

components/
home/
recipe/
learn/
watch/
recommendation/
sections/
layouts/
partials/
```

Each content type owns its templates and reusable sections.

---

# Components

```
components/

ui/
global/
```

UI contains reusable design system components.

Examples:

- badge
- button
- card
- section
- section-header

Global contains shared website components.

Examples:

- author-card
- share
- reading-progress
- back-to-top

---

# Home

Contains homepage sections.

Example:

- Hero
- Featured Recipes
- Categories
- Latest Learn
- Latest Watch
- Latest Recommendations

---

# Recipe

Contains recipe-specific templates.

Examples:

- Hero
- Ingredients
- Instructions
- Equipment
- FAQ
- Storage
- Related Recipes
- Video

---

# Learn

Contains educational article templates.

---

# Watch

Contains video content templates.

---

# Recommendation

Contains product recommendation templates.

---

# Philosophy

The project follows a modular architecture.

Each feature owns its:

- Templates
- Components
- Partial views

This keeps the code organized, reusable, and scalable.
