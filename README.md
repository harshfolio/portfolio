# Portfolio

Personal blog and portfolio site built with Hugo.

## Quick Start

### Local Development

```bash
# Start Hugo dev server
~/bin/hugo server -D

# Visit http://localhost:1313
```

### Writing a New Post

```bash
# Create a new post
~/bin/hugo new content/posts/my-new-post.md

# Or manually create: content/posts/my-new-post.md
```

**Post template:**

```markdown
---
title: "Your Post Title"
date: 2025-10-02
draft: false
math: true  # Enable if using LaTeX
tags: ["tag1", "tag2"]
---

Your content here...

## Math Example

Inline: $E = mc^2$

Display:
$$
\int_{-\infty}^{\infty} e^{-x^2} dx = \sqrt{\pi}
$$
```

## Deployment

**Automatic:** Push to `main` branch → GitHub Actions builds and deploys to GitHub Pages

**One-time setup required:**
1. Go to repository Settings → Pages
2. Source: **GitHub Actions**

## Project Structure

```
.
├── content/
│   ├── posts/          # Blog posts go here
│   └── about.md        # About page
├── static/
│   └── images/         # Images go here
├── themes/
│   └── PaperMod/       # Theme files
├── layouts/
│   └── partials/       # Custom layouts (KaTeX)
└── hugo.toml           # Site configuration
```

## Features

✅ Clean, minimal design (PaperMod theme)
✅ LaTeX/Math support (KaTeX)
✅ Syntax highlighting
✅ Dark mode
✅ Fast builds (Hugo)
✅ Auto-deploy to GitHub Pages

## Customization

- **Site settings:** Edit `hugo.toml`
- **Theme colors:** Edit `themes/PaperMod/` files
- **About page:** Edit `content/about.md`
- **Social links:** Update `hugo.toml` socialIcons section
