# Grilled Games Website

A static website built with Jekyll, hosted on GitHub Pages.

## Local Development

### Prerequisites
- Ruby 3.x (for Jekyll)
- Jekyll gem installed (`gem install jekyll`)

### Running Locally
```bash
jekyll serve
```

### Adding a Blog Post
Create a new file in `_posts/` with the format `YYYY-MM-DD-title.md`:
```markdown
---
title: "Your Title"
date: YYYY-MM-DD
categories: news
tags: [tag1, tag2]
---

Content here...
```

### Adding Games
Edit `_data/games.yml` to add or modify games. Each entry needs:
- `slug`: unique identifier
- `title`: display name
- `description`: short description
- `image`: path to image file (place images in `assets/img/`)
- `stripe_url`: Stripe checkout link

## GitHub Pages

This site is configured for GitHub Pages. Push to the main branch and GitHub will automatically build and host it.

## Features

- **Dark mode toggle**: Click the sun/moon icon in the header to switch between light and dark themes. Your preference is saved in localStorage.
- **Responsive design**: Works on desktop, tablet, and mobile devices.
- **Blog**: Powered by Jekyll's built-in blog functionality.
- **Store**: Physical thumb drives with games, linked via Stripe checkout.
