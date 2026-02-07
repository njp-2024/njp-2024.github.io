---
title: Portfolio Website
description: A responsive, multi-page portfolio site built with Jekyll and hosted on GitHub Pages.
tech:
  - Jekyll
  - SCSS
  - GitHub Pages
repo: "https://github.com/njp-2024/njp-2024.github.io"
live: "https://njp-2024.github.io"
order: 2
---

## Problem

A professional portfolio was needed to present projects and technical thinking to potential employers. The site needed to be fast, easy to maintain, and deployable at zero cost, while maintaining a modern and polished appearance.

## Approach

The site is built with Jekyll and hosted on GitHub Pages to keep the stack simple and deployment automatic. SCSS is used for modular styling, semantic HTML for accessibility, and a data-driven structure (YAML files for navigation and resume content) to separate content from presentation.

Project pages are structured as short technical briefs (Problem, Approach, Tradeoffs, Outcome) to emphasize clarity and reasoning.

## Tradeoffs

- **Jekyll vs. a JavaScript framework:** Jekyll provides a simpler, GitHub Pages–native workflow but offers less flexibility for dynamic interactivity. This was an acceptable tradeoff for a content-focused static site.
- **Built-in build process:** Relying on GitHub Pages’ Jekyll build limits plugin options but avoids the overhead of a custom CI/CD pipeline.
- **Minimal JavaScript:** JavaScript is used only for basic scroll-triggered animations; layout and interaction are handled primarily with HTML and CSS.

## Outcome

The result is a clean, fast portfolio that is easy to update and extend. New projects or posts can be added by creating a single markdown file, keeping ongoing maintenance low.
