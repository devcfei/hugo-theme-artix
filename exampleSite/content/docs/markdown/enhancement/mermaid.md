---
title: "Mermaid"
date: 2021-05-28T22:02:22+08:00
weight: 1
mdext:
    - mermaid

#draft: true
---


# Mermaid support

To enable mermaid, the mermaid for extention should be set.

**Example**

```yaml
---
mdext:
    - mermaid
---
```

There are two way to use mermaid
1. Use short code
1. Use markdown customized block

## Use shortcode

{{<mermaid>}}
graph LR;
	A[Hard edge] -->|Link text| B(Round edge)
    B --> C{Decision}
    C -->|One| D[Result one]
    C -->|Two| E[Result two]
{{< /mermaid >}}


**Shortcode**

```markdown
{{</*mermaid*/>}}
graph LR;
	A[Hard edge] -->|Link text| B(Round edge)
    B --> C{Decision}
    C -->|One| D[Result one]
    C -->|Two| E[Result two]
{{</* /mermaid */>}}
```

## Markdown customized block(WIP)



```mermaid
graph LR;
	A[Hard edge] -->|Link text| B(Round edge)
    B --> C{Decision}
    C -->|One| D[Result one]
    C -->|Two| E[Result two]
```

```markdown
```mermaid
graph LR;
	A[Hard edge] -->|Link text| B(Round edge)
    B --> C{Decision}
    C -->|One| D[Result one]
    C -->|Two| E[Result two]
```
```

