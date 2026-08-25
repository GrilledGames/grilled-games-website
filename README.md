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
- **Store**: Physical thumb drives with games, linked via Stripe checkout.
