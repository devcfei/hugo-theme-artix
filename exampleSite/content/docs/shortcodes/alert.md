---
title: "Alert"
date: 2021-05-30T10:19:48+08:00
weight: 3
#draft: true
---


# Alert

The `alert` shortcode allow you to highlight information in your page. They create a colored box surrounding your text, like this:

{{%alert%}}**This is** an alert !{{%/alert%}}

## Usage 

| Parameter | Default | Description |
|:--|:--|:--|
| theme | info | primary, success, info, warning, danger, dark, light, secondary |

{{%alert info%}}
**Tips :** setting only the theme as argument works too : 
`{{%/*alert warning*/%}}`  instead of `{{%/*alert theme="warning"*/%}}`
{{%/alert%}}

## Basic examples

```markdown
{{%/* alert primary */%}}**this** is a primary{{%/* /alert */%}}
{{%/* alert theme="info" */%}}**this** is a text{{%/* /alert */%}}
{{%/* alert theme="success" */%}}**Yeahhh !** is a text{{%/* /alert */%}}
{{%/* alert theme="warning" */%}}**Be carefull** is a text{{%/* /alert */%}}
{{%/* alert danger */%}}**Beware !** is a text{{%/* /alert */%}}
{{%/* alert dark */%}}**Dark !** is a dark{{%/* /alert */%}}
{{%/* alert light */%}}**oooh !** is a light{{%/* /alert */%}}
{{%/* alert secondary */%}}**Wait !** is a secondary{{%/* /alert */%}}
```
{{% alert primary %}}**this** is an primary{{% /alert %}}
{{% alert theme="info"%}}**this** is an info{{% /alert %}}
{{% alert theme="success" %}}**Yeahhh !** is a success{{% /alert %}}
{{% alert theme="warning" %}}**Be carefull** is a warning{{% /alert %}}
{{% alert danger %}}**Beware !** is a danger{{% /alert %}}
{{% alert dark %}}**Dark !** is a dark{{% /alert %}}
{{% alert light %}}**oooh !** is a light{{% /alert %}}
{{% alert secondary %}}**Wait !** is a secondary{{% /alert %}}