---
title: "Welcome to My Blog"
description: "A sample blog post demonstrating the features of this Hugo-powered blog with math, code highlighting, and more."
date: 2025-10-02
draft: false
math: true
tags: ["intro", "tutorial"]
---

## Hello World

This is a sample blog post demonstrating the features of this Hugo-powered blog.

## Math Support

You can write inline math like $E = mc^2$ or display equations:

$$
\int_{-\infty}^{\infty} e^{-x^2} dx = \sqrt{\pi}
$$

Here's another example with the quadratic formula:

$$
x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}
$$

## Code Highlighting

```python
def fibonacci(n):
    if n <= 1:
        return n
    return fibonacci(n-1) + fibonacci(n-2)

print(fibonacci(10))
```

```javascript
const greet = (name) => {
  console.log(`Hello, ${name}!`);
};

greet("World");
```

## Images

You can add images by placing them in the `static/images/` folder and referencing them like:

```markdown
![Alt text](/images/your-image.png)
```

## Markdown Features

- **Bold text**
- *Italic text*
- `inline code`
- [Links](https://gohugo.io)

1. Ordered lists
2. Work great
3. Too!

> Blockquotes are also supported for highlighting important information.

---

That's it! Start writing by adding markdown files to `content/posts/`.
