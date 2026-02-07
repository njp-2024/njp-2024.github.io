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

Needed a professional portfolio to showcase projects and technical thinking for potential employers. The site had to be fast, maintainable, and hostable at zero cost — while looking modern and polished.

## Approach

Built with Jekyll on GitHub Pages to keep the stack simple and deployment automatic. Used SCSS for modular styling, semantic HTML for accessibility, and a data-driven architecture (YAML files for resume and navigation) to separate content from presentation.

Structured project pages as technical briefs (Problem, Approach, Tradeoffs, Outcome) to demonstrate structured thinking.

## Tradeoffs

- **Jekyll vs. a JS framework:** Jekyll is simpler and GitHub Pages–native, but less flexible for interactivity. The right tradeoff for a content-first static site.
- **No build pipeline:** Relies on GitHub Pages' built-in Jekyll build. Limits plugin choices but eliminates CI/CD complexity.
- **Minimal JavaScript:** Only used for scroll-triggered animations. Everything else is CSS and HTML.

## Outcome

A clean, fast portfolio that's easy to maintain and extend. Adding a new project or blog post requires only creating a markdown file.
