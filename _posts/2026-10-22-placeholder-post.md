---
layout: post
title: Placeholder - how to write a post
date: 2026-10-22 12:00:00-0400
description: A placeholder post showing how to write a blog post, including how to include LaTeX math
tags: formatting math
categories: placeholder
related_posts: false
---

This is a placeholder post. Use it as a template: copy the file, or edit it in place and replace the text.

## Creating a post

1. Add a Markdown file to `_posts/` named `YYYY-MM-DD-your-title.md`. The date in the filename sets the post date.
2. Fill in the front matter at the top of the file, between the two `---` lines: `layout: post`, `title`, `date`, `description`, and optionally `tags` and `categories`.
3. Write the body below the second `---` in ordinary Markdown.
4. Preview locally with `bundle exec jekyll serve`, then open `http://localhost:4000`.

Posts are published at `/blog/YEAR/TITLE/`, using the `permalink` set in `_config.yml`.

## Markdown basics

Headings, _italic_, **bold**, [links](https://example.com), and lists all work as usual.

- a bullet point
- another bullet point

Code blocks use triple backticks and a language name:

```python
import pandas as pd
```

## Images

Put the image file in `assets/img/`, then embed it with the figure include, passing the `path`, `title`, and `class` attributes. The example below sits inside a raw block so it displays as text rather than rendering the image:

{% raw %}
```liquid
{% include figure.liquid path="assets/img/prof_pic.jpg" title="a caption" class="img-fluid rounded z-depth-1" %}
```
{% endraw %}

## LaTeX math

Math is enabled site-wide (`enable_math: true` in `_config.yml`) and rendered with MathJax.

Inline math sits inside a sentence, for example the identity $$ E = mc^2 $$ or the sample mean $$ \bar{x} = \frac{1}{n}\sum_{i=1}^{n} x_i $$.

Display math goes on its own line, between `$$` markers:

$$
\hat{\beta} = (X^\top X)^{-1} X^\top y
$$

Numbered equations use the `equation` environment, and a `\label` lets you refer to them with `\eqref`:

\begin{equation}
\label{eq:gaussian}
f(x) = \frac{1}{\sqrt{2\pi\sigma^2}} \exp\left(-\frac{(x-\mu)^2}{2\sigma^2}\right)
\end{equation}

Equation \eqref{eq:gaussian} is the Gaussian density.

### Tips

- Math needs no special escaping in the post body. Write `\frac`, `\sum`, and so on as they appear in LaTeX.
- If a section contains Liquid-style curly braces, wrap it in a raw block as shown in the Images section above.
- To show LaTeX as text instead of rendering it, put it in a code block.
