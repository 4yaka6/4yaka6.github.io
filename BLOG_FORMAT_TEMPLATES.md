# Blog Format Templates

## Standard Post

```md
---
layout: post
title: Your Title
excerpt: A short summary shown on listing pages.
tags:
  - tag-one
  - tag-two
author: Your Name
date: 2026-04-17 20:00 +0800
permalink: /blog/your-slug/
toc: true
math: false
ifhide: false
---

Intro paragraph.

## Section Title

Normal paragraph text.
```

## Standard Math

Inline formula:

```md
The formula is $a^2 + b^2 = c^2$.
```

Display formula:

```md
$$
\operatorname{Attention}(Q, K, V) = \operatorname{softmax}\left(\frac{QK^T}{\sqrt{d_k}}\right)V
$$
```

Alternative inline formula:

```md
The formula is \(a^2 + b^2 = c^2\).
```

## Standard Code Block

Without line numbers:

~~~~md
```python
def hello():
    print("hello")
```
~~~~

With Rouge line numbers:

~~~~md
{% highlight python linenos %}
def hello():
    print("hello")
{% endhighlight %}
~~~~

## Standard Quote And Note

```md
> This is a quote block.

Important note here.
{: .message }
```

## Hidden Post

For complete hiding in this repo, keep both `ifhide: true` and `hidden: true`.
`ifhide` is used by the theme templates.
`hidden` is used by `jekyll-paginate` so the post is excluded from homepage pagination.

```md
---
layout: post
title: Hidden Post
date: 2026-04-17 20:00 +0800
permalink: /hidden/your-secret-post/
ifhide: true
hidden: true
sitemap: false
math: false
toc: false
---

Hidden content here.
```

## Minimal Hello Example

```md
---
layout: post
title: hello
date: 2026-04-17 20:00 +0800
permalink: /hidden/hello/
ifhide: true
hidden: true
sitemap: false
math: false
toc: false
---

hello
```
