---
title: Markdown 扩展功能
published: 2024-05-01
updated: 2024-11-29
description: '阅读更多关于 Fuwari 中 Markdown 功能的内容'
image: ''
tags: [Demo, Example, Markdown, Fuwari]
category: 'Examples'
draft: false 
---

## GitHub 仓库卡
您可以添加链接到 GitHub 存储库的动态卡片，页面加载时，存储库信息将从 GitHub API 获取。

::github{repo="Fabrizz/MMM-OnSpotify"}

创建一个包含代码的 GitHub 仓库卡片 `::github{repo="<owner>/<repo>"}`.

```markdown
::github{repo="saicaca/fuwari"}
```

## 提示

支持以下类型的提示: `note`  `tip`  `important`  `warning`  `caution`

:::note
有用的信息，用户在浏览内容时应该知道。
:::

:::tip
提供更好或更容易做事的有益建议。
:::

:::important
用户为了实现目标所需的关键信息。
:::

:::warning
紧急信息，需要用户立即注意以避免问题。
:::

:::caution
关于某些操作的风险或负面结果的建议。
:::

### 基本语法

```markdown
:::note
Highlights information that users should take into account, even when skimming.
:::

:::tip
Optional information to help a user be more successful.
:::
```

### 自定义标题

警告标题可以自定义。

:::note[我的自定义标题]
这是一个带有自定义标题的注释。
:::

```markdown
:::note[我的自定义标题]
这是一个带有自定义标题的注释。
:::
```

### GitHub语法

> [!TIP]
> [GitHub语法](https://github.com/orgs/community/discussions/16925) 语法也受支持。

```
> [!NOTE]
> The GitHub syntax is also supported.

> [!TIP]
> The GitHub syntax is also supported.
```

### Spoiler 隐藏文字

你可以给你的文本添加 spoiler。Spoiler内也支持 Markdown 语法。

内容:spoiler[被隐藏了 **ayyy**]!

```markdown
内容:spoiler[被隐藏了 **ayyy**]!

```