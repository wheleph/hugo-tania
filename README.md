# Hugo Theme Tania

A simple theme for bloggers.

## Demo

[Example Site](https://hugo-tania.netlify.app/)

[![Netlify Status](https://api.netlify.com/api/v1/badges/bae5db51-7cc6-41e2-9615-029ade8aa264/deploy-status)](https://app.netlify.com/sites/hugo-tania/deploys)

## Introduction
Most of the styles for this theme come from [taniarascia.com](https://github.com/taniarascia/taniarascia.com)

I like it's style, so I transplant it to Hugo.

And is that why this theme called Tania.

Thank Tania Rascia again.

## Features

- Dark mode(It can switch automatically or manually)
- Footnotes(Float on the right side)
- Search with categories filter

## Usage

### Installation

In your site's root dir

```bash
git submodule add https://github.com/WingLim/hugo-tania themes/hugo-tania
```

Edit your site config following `exampleSite/config.yaml`.

### Params

`titleEmoji` will show before the blog title on site navbar.

```yaml
titleEmoji: '😎'
```

`socialOptions` will show on index bio with `_index.md` content.
Account with icon can set as below:
```yaml
socialOptions:
    dev-to:
    email:
    facebook:
    github:
    instagram:
    linkedin:
    medium:
    stack-overflow:
    steam:
    telegram:
    twitter:
    twitch:
    whatsapp:
```

If you want to disable the float footnotes, add below params.
```yaml
enableFootnotes: false
```

Limit how many categories filter show above search input.

Default is `5`
```yaml
maxCategoryToShow: 10
```

### Layout

`articles` layout is for showing all articles you write.

Add `articles.md` to site `content` dir, and write as below:

```markdown
---
title: Articles
subtitle: Posts, tutorials, snippets, musings, and everything else.
date: 2020-11-26
type: section
layout: "archives"
---
```

### Article

#### Enable math formula render

For enable math formula render, add `katex: true` or `mathjax: true` in your article head, like:

Notice: You should enable only one `katex` or `mathjax` in a same time.

```markdown
---
title: Title
katex: true
---

Some content...

```

## Thanks to
- [你好黑暗，我的老朋友 —— 为网站添加用户友好的深色模式支持](https://blog.skk.moe/post/hello-darkmode-my-old-friend/)
- [Footnotes, citations, and sidenotes](https://prose.yihui.org/about/#footnotes-citations-and-sidenotes)

## License

[MIT](https://github.com/WingLim/hugo-tania/blob/main/LICENSE)