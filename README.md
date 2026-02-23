# Chibi Gen Studio — Website

A modern Jekyll website for Chibi Gen Studio, built for GitHub Pages.

## Features

- **Blog system** with YouTube embed and image support
- **Gumroad & Superhive** buy button integration
- **Responsive design** — looks great on desktop and mobile
- **Dark theme** with a modern, clean aesthetic
- **SEO-friendly** with jekyll-seo-tag and sitemap

## Quick Start

### Prerequisites
- [Ruby](https://www.ruby-lang.org/) 2.7+
- [Bundler](https://bundler.io/)

### Local Development

```bash
bundle install
bundle exec jekyll serve
```

Then open [http://localhost:4000](http://localhost:4000) in your browser.

### Deploy to GitHub Pages

1. Push this repo to GitHub
2. Go to **Settings → Pages**
3. Set source to the `main` branch
4. Your site will be live at `https://yourusername.github.io/repo-name/`

## Adding a Blog Post

Create a new file in `_posts/` with the naming convention:

```
YYYY-MM-DD-your-post-title.md
```

### Front Matter Options

```yaml
---
layout: post
title: "Your Post Title"
date: 2026-02-20
categories: [Tutorials]
excerpt_text: "Short description for the blog list."
image: /assets/images/your-image.png
gumroad_id: your-product-id        # optional: adds Gumroad buy button
superhive_url: https://example.com  # optional: adds Superhive buy button
---
```

### Embedding YouTube Videos

```liquid
{% include youtube.html id="VIDEO_ID" title="Video Title" %}
```

### Adding Buy Buttons Inside Posts

```liquid
{% include gumroad_button.html id="product-id" text="Buy on Gumroad — $29" %}
{% include superhive_button.html url="https://superhive.example.com/product" text="Buy on Superhive — $29" %}
```

## Configuration

Edit `_config.yml` to customize:
- Site title, description, URL
- Author info and social links
- Footer details

## License

© 2026 Chibi Gen Studio. All rights reserved.
