# FLVRTX Deployment Guide

This document describes the deployment process for the FLVRTX website from local development to production.

---

# Environment

## Local Development

- LocalWP
- PHP
- WordPress
- Sage 11
- Node.js
- Composer

---

## Production

- Hostinger
- LiteSpeed Server
- SSL Enabled
- PHP 8.3+
- MySQL

---

# Development Workflow

## Install Dependencies

```bash
composer install
npm install
```

---

## Start Development

```bash
npm run dev
```

---

## Production Build

Before deployment:

```bash
npm run build
```

This generates optimized assets.

---

# Deployment Steps

1. Commit latest changes

```bash
git add .
git commit -m "Release"
git push
```

---

2. Build production assets

```bash
npm run build
```

---

3. Upload theme

Upload the compiled theme to:

```
wp-content/themes/flvrtx-theme
```

---

4. Activate Theme

Appearance

↓

Themes

↓

FLVRTX Theme

---

5. Clear Cache

- LiteSpeed Cache
- Browser Cache
- CDN (if applicable)

---

6. Verify Website

Check:

- Homepage
- Recipes
- Learn
- Watch
- Recommendations
- Search
- 404

---

# Production Checklist

Before launch:

- Build completed
- SSL enabled
- Images optimized
- Sitemap working
- Robots.txt verified
- Search Console connected
- Analytics connected
- Cache enabled
- Backups configured

---

# Rollback

If deployment fails:

1. Restore previous backup.

2. Restore previous database.

3. Clear caches.

4. Verify website.

---

# Future Improvements

- CI/CD
- GitHub Actions
- Automatic deployments
- Staging environment

---

# Goal

Every deployment should be repeatable, reliable, and fully documented.
