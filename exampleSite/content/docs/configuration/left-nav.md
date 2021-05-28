---
title: "Left Navigator"
date: 2021-05-27T21:40:09+08:00
layouts:
    - nav
weight: 3
#draft: true
---



# Navigator on the left

## Enable the Navigator

```yml
layouts:
    - nav         # Enable Left Navigator 
```

`alwaysNav` in `config.toml` enable all the Breadcrumb even `nav` is not set in `layouts`

```toml
[params]
alwaysNav = true    # always have navigator for a page
```

## Exclude the folder

The nav_exclusion list in `config.toml` helps to hide the folders in Navigator

```toml
# path name excluded from documentation navigator
nav_exclusion = [
    "articles",
]
```

## Customize the Navigator

To customize the Navigator, change the default setting of `ul, li in main-nav` in `static/css/style.css`  

```css
.main-nav{
    max-width: 20rem;
    min-width: 20rem;
    /* background-color:rgb(164, 243, 245); */
    border-right:1px dashed  #E7E7E7;

}

.main-nav ul
{
    padding-left: 1em;
    margin: 0;
    padding: 0;
    list-style: none;
    user-select: none;    
    padding-left: 0px;  

}

.main-nav ul li{
    margin: 10 0;
    padding-left: 1em;
    list-style: none;
    user-select: none;
}

```




