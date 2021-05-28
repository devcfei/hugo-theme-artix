---
title: "Breadcrumb"
date: 2021-05-27T21:41:01+08:00
weight: 5
layouts:
    - toc
    - breadcrumb
#draft: true
---


# Breadcrumb on the top of the article

## Enable the Breadcrumb

```yml
layouts:
    - breadcrumb         # Enable Breadcrumb 
```

`alwaysBreadcrumb` in `config.toml` enable all the Breadcrumb even `breadcrumb` is not set in `layouts`

```toml
[params]
alwaysBreadcrumb = true    # always have TOC for a page
```


## Customize the Breadcrumb

To customize the Breadcrumb, change the default setting of `ul, li in nav-breadcrumb` in `static/css/style.css`  

```css
.nav-breadcrumb ul{
    padding: 0px 0px;
    margin-bottom: 20px;
    list-style: none;
    background-color: #fafafa;
}

.nav-breadcrumb ul> li {
    display: inline-block;
}

.nav-breadcrumb ul > li + li:before {
    padding: 0px 0px;
    color: #1c495f;
    content: "/\00a0";
}

.nav-breadcrumb ul > .active {
    color: #777;
}

```

