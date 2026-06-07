# rootaccess.blog — Jekyll Theme

Terminal-aesthetic Jekyll blog. Dark, readable, no fluff.

## Setup

```bash
# Install dependencies
bundle install

# Run locally
bundle exec jekyll serve

# Build for production
bundle exec jekyll build
```

Site builds to `_site/`. Point Apache at that directory.

## Writing a post

Create a file in `_posts/` named `YYYY-MM-DD-post-title.md`:

```markdown
---
layout: post
title: "Your Post Title"
date: 2024-06-01 00:00:00 -0600
tags: [linux, security]
excerpt: "One sentence summary shown on the homepage."
---

Your content in Markdown here.
```

## Deploy (Lightsail / Apache)

Drop your `deploy.sh` workflow here — `git pull` → `bundle exec jekyll build` → copy `_site/` to your Apache document root.

```bash
#!/bin/bash
cd /var/www/rootaccess
git pull origin main
bundle exec jekyll build
sudo cp -r _site/. /var/www/html/
```

## Tags

Tag pages are generated automatically. Use consistent lowercase tags.
Suggested: `infrastructure`, `security`, `linux`, `networking`, `how-to`, `homelab`, `misc`

## Structure

```
rootaccess/
├── _config.yml          # Site config
├── _layouts/
│   ├── default.html     # Base layout (header + footer)
│   ├── post.html        # Single post page
│   └── tag.html         # Tag filter page
├── _posts/
│   └── YYYY-MM-DD-*.md  # Your posts go here
├── assets/
│   └── css/
│       └── main.css     # All styles
├── index.html           # Homepage
└── Gemfile
```
