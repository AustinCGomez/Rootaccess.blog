# rootaccess.blog — Terminal Dark Theme

A terminal-inspired Jekyll theme for rootaccess.blog.

## Files

```
_config.yml               ← site-wide settings (update author info)
_layouts/
  default.html            ← base layout (head + nav + footer)
  home.html               ← post listing index
  post.html               ← single post view
  page.html               ← standalone pages
_includes/
  head.html               ← <head> meta, fonts, CSS link
  header.html             ← window chrome + terminal nav
  footer.html             ← site footer
_sass/
  rootaccess.scss         ← all styles (single file)
assets/css/
  main.scss               ← SCSS entry point (imports _sass/rootaccess)
about.md                  ← About page — edit with your real info
index.html                ← Home page (uses home layout)
Gemfile                   ← Ruby dependencies
_posts/
  2025-11-14-proxmox-homelab-setup.md   ← example post
```

## Setup

### Fresh start
```bash
bundle install
bundle exec jekyll serve
```

### Drop into existing site
1. Copy `_layouts/`, `_includes/`, `_sass/`, `assets/` into your repo root
2. Replace your `_config.yml` with this one (or merge the settings)
3. Replace `index.html` with the new one
4. Add `about.md` to your repo root
5. Run `bundle install && bundle exec jekyll serve`

## Customising

### _config.yml — update these fields
```yaml
title:   rootaccess          # blog name (shown in nav prompt)
tagline: "IT notes from..."  # shown in hero subtitle
url:     "https://rootaccess.blog"

author:
  name:   "Your Name"
  handle: "yourhandle"       # used in the shell prompt: yourhandle@rootaccess:~ $
  email:  "you@rootaccess.blog"
  github: "yourhandle"
```

### about.md
Replace the placeholder copy, skills, and contact links with your real details.
The avatar initials (`RA`) are hardcoded in the HTML — change them to your initials.

### Post tags
Tags drive the coloured badges on the index and post pages.
Supported out of the box: `linux`, `devops`, `security`, `networking`, `homelab`, `windows`, `cloud`

To add a new tag, add a rule to `_sass/rootaccess.scss` in the `.post-tag` block:

```scss
&.mynewcategory { color: #xyz; background: rgba(x,y,z,0.08); border-color: rgba(x,y,z,0.2); }
```

### Post front matter
```yaml
---
layout: post
title:  "Your post title"
date:   2025-11-14
tags:   [linux]           # first tag shown as badge on index
description: "One-line summary shown under the title"
---
```

## Rouge syntax highlighting
The theme uses Rouge (built into Jekyll). Code blocks in posts are automatically
highlighted. The terminal-style left green border is applied via CSS — no extra
config needed.
