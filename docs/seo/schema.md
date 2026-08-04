# FLVRTX Schema Documentation

This document describes the structured data (Schema.org) implementation used throughout FLVRTX.

---

# Purpose

Structured data helps search engines understand page content and enables rich search results.

FLVRTX uses JSON-LD wherever possible.

---

# Schema Types

## Organization

Represents the FLVRTX brand.

Includes:

- Name
- Logo
- Website
- Social Profiles

---

## WebSite

Represents the entire website.

Includes:

- Website Name
- URL
- Search Action (future)

---

## BreadcrumbList

Every public page should expose breadcrumb schema.

Example:

Home

↓

Recipes

↓

Chicken Curry

---

## Recipe

Recipe pages include:

- Name
- Description
- Featured Image
- Author
- Prep Time
- Cook Time
- Total Time
- Servings
- Ingredients
- Instructions
- Nutrition (future)
- Video (when available)

Current implementation:

app/View/Composers/RecipeSchema.php

---

## Article

Used for Learn pages.

Includes:

- Headline
- Description
- Author
- Date Published
- Featured Image

---

## VideoObject

Used on Watch pages.

Includes:

- Video Title
- Description
- Thumbnail
- Upload Date
- Embed URL

---

## Product

Future implementation for Recommendation pages.

Includes:

- Product Name
- Brand
- Image
- Description
- Rating
- Price
- Availability

---

# Validation

Validate structured data using:

Google Rich Results Test

Schema Markup Validator

---

# Best Practices

- Never generate invalid JSON.
- Keep schema synchronized with page content.
- Avoid duplicate schema.
- Include only relevant properties.

---

# Future Improvements

- FAQ Schema
- HowTo Schema
- Product Schema
- Organization Social Profiles
- SearchAction

---

# Goal

Every page should expose clean, valid, and useful structured data to improve search visibility and rich search experiences.
