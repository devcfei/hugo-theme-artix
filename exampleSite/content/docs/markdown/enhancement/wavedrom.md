---
title: "Wavedrom"
date: 2021-05-28T22:40:22+08:00
weight: 3
mdext:
    - wavedrom
#draft: true
---



# Wavedrom support


To enable Wavedrom, the wavedrom for extention should be set.

**Example**

```yaml
---
mdext:
    - wavedrom
---
```

There are two way to use Wavedrom
1. Use short code
1. Use markdown customized block

## Use shortcode

{{< wavedrom>}}
{ 
  "signal": [ {"name": "CLK", "wave": "p.....|..."},
            {"name":"DAT", "wave":"x.345x|=.x", "data":["A","B","C","D"]},
            {"name": "REQ", "wave": "0.1..0|1.0"},
            {},
            {"name": "ACK", "wave": "1.....|01."}
]}
{{< /wavedrom >}}



**Shortcode**

```markdown
{{</* wavedrom */>}}
{ 
  "signal": [ {"name": "CLK", "wave": "p.....|..."},
            {"name":"DAT", "wave":"x.345x|=.x", "data":["A","B","C","D"]},
            {"name": "REQ", "wave": "0.1..0|1.0"},
            {},
            {"name": "ACK", "wave": "1.....|01."}
]}
{{</* /wavedrom */>}}
```


## Markdown customized block(WIP)



```wavedrom
{ 
  "signal": [ {"name": "CLK", "wave": "p.....|..."},
            {"name":"DAT", "wave":"x.345x|=.x", "data":["A","B","C","D"]},
            {"name": "REQ", "wave": "0.1..0|1.0"},
            {},
            {"name": "ACK", "wave": "1.....|01."}
]}
```

```markdown
```wavedrom
{ 
  "signal": [ {"name": "CLK", "wave": "p.....|..."},
            {"name":"DAT", "wave":"x.345x|=.x", "data":["A","B","C","D"]},
            {"name": "REQ", "wave": "0.1..0|1.0"},
            {},
            {"name": "ACK", "wave": "1.....|01."}
]}
```
```

