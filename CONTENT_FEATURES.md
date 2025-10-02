# Content Enhancement Features

This document explains how to use the advanced content features in your blog.

## Table of Contents

Automatic table of contents will appear on posts with enough content (>100 characters in TOC).

**Features:**
- Sticky positioning on desktop (floats right)
- Active section highlighting as you scroll
- Automatically generated from H2 and H3 headings
- Mobile-responsive (moves to top on smaller screens)

**Usage:**
Just write your post with H2 and H3 headings - the TOC generates automatically!

```markdown
## Main Section
Content here...

### Subsection
More content...
```

## Related Posts

Related posts appear at the bottom of each post, using Hugo's built-in related content algorithm based on tags.

**Shows:**
- Up to 3 related posts
- Title, description, date, and reading time
- Hover effects for better UX

**Usage:**
Add tags to your post frontmatter:

```yaml
---
title: "My Post"
tags: ["data engineering", "analytics", "dbt"]
---
```

## Footnotes & Sidenotes

### Standard Footnotes

Use standard Markdown footnote syntax:

```markdown
This is a statement that needs a citation[^1].

[^1]: This is the footnote content.
```

Footnotes will appear at the bottom of the post with proper styling.

### Sidenotes (Gwern-style)

For important side comments that should be visible inline:

```html
<span class="sidenote">
This is a side comment that will appear in the margin on desktop,
and inline on mobile.
</span>
```

**Best for:**
- Technical clarifications
- Additional context
- Tangential but important information

## Code Blocks with Language Labels

Code blocks automatically show language labels in the top-right corner.

**Usage:**

````markdown
```python
def hello_world():
    print("Hello, World!")
```
````

The language label will appear automatically based on the code fence language specifier.

**Supported:**
All languages supported by Hugo's syntax highlighter (Python, JavaScript, Go, Rust, SQL, etc.)

## Post Frontmatter Template

```yaml
---
title: "Your Post Title"
description: "Brief description that appears in post list and related posts"
date: 2025-03-23
draft: false
tags: ["tag1", "tag2", "tag3"]
---

## Introduction

Your content here...
```

## Tips for Best Results

1. **TOC**: Use descriptive H2/H3 headings - they become your TOC navigation
2. **Related Posts**: Use 3-5 relevant tags per post for better matching
3. **Footnotes**: Keep them concise - they're for citations and brief clarifications
4. **Sidenotes**: Use sparingly for maximum impact
5. **Code**: Always specify the language for proper highlighting and labeling
