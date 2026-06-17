---
title: Building This Site with Astro and Fuwari
published: 2026-06-17
description: Notes on the stack and deployment path for this GitHub Pages blog.
tags: [Astro, Fuwari, GitHub Pages]
category: Engineering
draft: false
lang: en
---

This site uses [Astro](https://astro.build/) with the [Fuwari](https://github.com/saicaca/fuwari) theme as its base.

## Stack

- Astro for static rendering.
- Fuwari for the blog system, page transitions, search, RSS, theme color controls, archive, tags, and responsive layout.
- GitHub Actions for building and deploying to GitHub Pages.

## Deployment Shape

The target repository is a user Pages repository named:

```text
dcygtheshy.github.io
```

For a user Pages site, Astro does not need a `base` path. The site URL should become:

```text
https://dcygtheshy.github.io/
```

## TODO Before Publishing

- Replace the avatar and banner with real assets if needed.
- Push the repository to GitHub and enable Pages with GitHub Actions.
