# FLVRTX Git Workflow

This document defines the Git workflow used for FLVRTX development.

---

# Repository Structure

FLVRTX consists of multiple repositories.

## flvrtx-theme

Contains the WordPress theme source code.

Includes:

- Blade templates
- PHP
- JavaScript
- CSS
- Assets

---

## flvrtx-os

Contains project documentation.

Includes:

- Architecture
- Design System
- Coding Standards
- Content Models
- Deployment Guides
- Roadmaps

---

# Branch Strategy

Main branch:

main

Future branches:

feature/<feature-name>

Examples:

feature/cook-mode

feature/dark-mode

feature/search-improvements

---

# Commit Messages

Follow Conventional Commits.

## Feature

feat: add recipe hero component

---

## Fix

fix: correct mobile navigation

---

## Documentation

docs: add deployment guide

---

## Refactor

refactor: modularize javascript

---

## Performance

perf: optimize hero images

---

## Style

style: improve spacing on recipe cards

---

# Development Workflow

1. Pull latest changes

git pull

---

2. Create feature branch

git checkout -b feature/new-feature

---

3. Develop feature

---

4. Commit changes

git add .

git commit -m "feat: add new feature"

---

5. Push branch

git push origin feature/new-feature

---

6. Create Pull Request

Review

Merge

Delete feature branch

---

# Releases

Release versions follow Semantic Versioning.

Examples:

v1.0.0

v1.1.0

v2.0.0

---

# Tags

Important releases should be tagged.

Example:

git tag v1.0.0

git push origin v1.0.0

---

# Backup Strategy

Always push code before:

- Major refactors
- Plugin updates
- Theme updates
- Production deployment

---

# Goal

Maintain a clean, traceable, and reliable version history throughout the FLVRTX project.
