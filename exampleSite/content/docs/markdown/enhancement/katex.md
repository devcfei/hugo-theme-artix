---
title: "KaTeX"
date: 2021-05-28T22:27:35+08:00
weight: 2
mdext:
    - katex
#draft: true
---

# KaTeX support

KaTeX let you to render math typesetting in markdown document. See [KaTeX](https://katex.org/)

To enable KaTeX, the katex for extention should be set.

**Example**

```yaml
---
mdext:
    - katex
---
```

There are two way to use KaTeX
1. Use short code
1. Use markdown customized block

## Use shortcode

{{< katex>}}
f(x) = \int_{-\infty}^\infty\hat f(\xi)\,e^{2 \pi i \xi x}\,d\xi
{{< /katex >}}



**Shortcode**

```markdown
{{</* katex*/>}}
f(x) = \int_{-\infty}^\infty\hat f(\xi)\,e^{2 \pi i \xi x}\,d\xi
{{</* /katex */>}}
```


## Markdown customized block(WIP)



```katex
f(x) = \int_{-\infty}^\infty\hat f(\xi)\,e^{2 \pi i \xi x}\,d\xi
```

```markdown
```katex
f(x) = \int_{-\infty}^\infty\hat f(\xi)\,e^{2 \pi i \xi x}\,d\xi
```
```
