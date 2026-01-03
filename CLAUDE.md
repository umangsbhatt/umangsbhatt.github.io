# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

Personal academic website for Umang Bhatt, built with Jekyll 2.5.3 using the Minimal Mistakes theme. Hosted on GitHub Pages at https://umangsbhatt.github.io.

## Build Commands

```bash
# Install Ruby dependencies
bundle install

# Serve locally with live reload
bundle exec jekyll serve

# Build for production
bundle exec jekyll build
```

### Grunt Tasks (for asset optimization)

```bash
# Install Node dependencies first
npm install

# Default: clean, uglify JS, optimize images
grunt

# Watch JS files and rebuild on changes
grunt dev

# Optimize images only
grunt images
```

## Architecture

- **Jekyll 2.x site** using Kramdown markdown and Rouge syntax highlighting
- **Theme**: Minimal Mistakes (two-column responsive layout)
- **Content files**: Markdown files with YAML front matter (index.md, research/index.md, contact/index.md)
- **Configuration**: `_config.yml` contains site settings, owner info, and social links
- **Layouts**: `_layouts/` (page.html, home.html, post.html, etc.)
- **Partials**: `_includes/` (navigation, footer, head, social sharing)
- **Styles**: `_sass/` with compressed CSS output
- **Assets**: `assets/js/` for JavaScript, `images/` for images

## Key Files

- `_config.yml` - Site configuration and owner metadata
- `index.md` - Homepage with bio, publications, and group members
- `research/index.md` - Research page
- `contact/index.md` - Contact page
