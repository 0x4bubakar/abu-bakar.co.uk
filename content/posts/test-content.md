+++
date = '2026-11-06T03:51:26Z'
title = 'Test Article'
tags = ["test", "markdown"]
categories = ["Misc"]
+++

This post is designed to test **Hugo's Goldmark Markdown renderer** and your theme's styling. Use it to check typography, alignment, color schemes, and media embeds.

---

## Typography & Inline Elements

Here is a standard paragraph containing various inline styles:

* **Bold text** to emphasize key points.
* *Italicized text* for emphasis or titles.
* ***Bold and italicized*** for strong emphasis.
* ~~Strikethrough text~~ for deprecated items.
* Inline `code blocks` using backticks.
* A [hyperlink to Hugo's official docs](https://gohugo.io/).

> **Blockquote:** "Perfection is achieved, not when there is nothing more to add, but when there is nothing left to take away."  
> — *Antoine de Saint-Exupéry*

---

## Lists

### Unordered List
- System Architecture
  - Frontend Interface
  - API Gateway
  - Database Layer
- Security & Authentication
- Deployment Pipeline

### Ordered List
1. Initialize the Hugo site: `hugo new site my-blog`
2. Add a theme via Git submodules.
3. Configure `hugo.toml` (or `config.toml`).
4. Run the local dev server: `hugo server -D`

### Task List
- [x] Configure Hugo Goldmark options
- [x] Test responsive CSS banner layout
- [ ] Deploy site to production

---

## Code Syntax Highlighting

Below is a fenced code block with syntax highlighting enabled.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Hugo Test</title>
    <link rel="stylesheet" href="/css/style.css">
</head>
<body>
    <header class="blog-banner-container">
        <img class="blog-banner" src="banner.jpg" alt="Blog Banner">
        <div class="banner-watermark">MY BLOG</div>
    </header>
</body>
</html>
```

```python3
def calculate_aspect_ratio(width: int, height: int) -> float:
    """Calculate decimal aspect ratio from dimensions."""
    if height == 0:
        raise ValueError("Height cannot be zero.")
    return round(width / height, 2)

print(f"800x140 aspect ratio: {calculate_aspect_ratio(800, 140)}:1")
```

Hugo Built-in Shortcodes

{{< figure src="https://images.unsplash.com/photo-1498050108023-c5249f4df085" alt="Laptop on desk with code" caption="A standard Hugo figure shortcode with caption." class="blog-banner" >}}
{{< youtube njX2bu-_Vw4 >}}

Here is a sentence with a footnote reference[^1].

[^1]: This is the footnote text detailing extra technical specifications

<ElicitationsGroup message="To take this further:">
  <Elicitation label="Add KaTeX mathematical equation syntax to the post" query="Update the Hugo test post to include examples of KaTeX mathematical equations and syntax."/>
  <Elicitation label="Add custom Hugo callout and alert shortcodes" query="Add examples of custom Hugo callout, warning, and alert shortcodes to the markdown test post."/>
</ElicitationsGroup>