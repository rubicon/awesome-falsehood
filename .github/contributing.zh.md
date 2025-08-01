# 贡献指南

欢迎您的贡献！以下是一些指导原则。

## 状态

这个仓库已经达到了平衡状态。我们已经过了积累阶段，正处于策展过程中。这意味着我们更注重完善概念、平滑进展以及仔细评估新内容的添加。

## 拉取请求和问题

- 在提出新建议之前，搜索过去和当前的问题和拉取请求。您的建议可能是重复的或正在进行中的工作。

- 每次提交只包含一个列表项。

- 每个拉取请求只包含一次提交。应用更改后始终压缩提交。

- 检查您的拼写和语法。

- 添加链接资源很棒的原因。以及它为现有内容增加了什么。

- 保持翻译内容与您的提议同步。将更改传播到所有 `readme.*.md` 文件。依赖自动翻译工具。双语贡献者稍后会完善结果。

## 代码检查

您的拉取请求应该通过 [官方 Awesome List 的检查器](https://github.com/sindresorhus/awesome-lint)。

这里不需要额外的工作，因为它已经 [通过 GitHub actions 集成](https://github.com/kdeldycke/awesome-falsehood/tree/main/.github/workflows)。

您仍然可以通过本地运行检查器来预测问题：

```shell-session
$ npx awesome-lint
```

## 格式化

以下是 `awesome-lint` CLI 未涵盖的其他规则。

如果这些规则中的任何一个与检查器冲突，检查器的规则应该优先。应用它们。

### 一般内容

- 删除任何尾随空格。

- 使用空格，不要使用制表符进行缩进。

- 撇号应使用单个 ASCII 标记：`'`。

- 对于描述，尝试从原始内容中识别最好的引用。

- 如果找不到引用作为摘要，请随意改写项目的标题和描述。记住，这是策展：我们通过聚合和分类来增加原始内容的价值。还通过智能编辑。您只需要尊重原始内容的精神。

### 章节

- 章节 **不是故意按字母顺序排序的**。这是为了提供从一般到特定主题的进展。

> [!IMPORTANT]
> 例外情况是在 `awesome-falsehood` 中，章节 **按字母顺序排列**，因为所有主题彼此独立。

- 章节可能包含一段介绍和一个图形（图表、绘图、照片）。

### URL

- 如果可用，使用 HTTPS 协议。

- 必须可被 CI/CD 作业访问。如果域名因速率限制或内容保护而返回 `40x` 错误，请用稳定链接替换：

  - [`sci-hub.st`](https://sci-hub.st) 用于研究论文
  - [`archive.ph`](https://archive.ph) 用于新闻文章
  - [`archive.org`](https://archive.org) 用于其他任何内容

### 项目标题

- 不使用 `"` 和 `"` 弯引号。这些保留用于描述中的原始内容引用。

- 要引用，使用单引号或双引号变体：`'` 和 `"`。保持它们适当平衡。

> [!IMPORTANT]
> 在 `awesome-falsehood` 中，链接标题必须删除 "*程序员认为*" 部分以保持紧凑。

### 项目描述

- 尝试提供可操作的 TL;DR 作为描述，如果原文能够独立存在，则引用原文。

- [删除描述中的 `TL;DR:` 前缀](https://github.com/kdeldycke/awesome-engineering-team-management/commit/da298ec1c39fe62fd4553e1a6de0ad4494602c57)。每个描述都是简短摘要。

- 引用应该用 `"` 和 `"` 弯引号正确分隔。

- 您可以使用括号中的省略号 `(…)` 来缩减原文。

- 对于引用内的引用，使用单引号或双引号 `'` 和 `"` ASCII 标记。保持它们适当平衡。

- 要将列表序列化为描述，使用以下格式：

  > 总结项目的描述文本。这里是来自原始内容的列表，关于 **"三个重要主题：1. 某某某；2. 某某某？3. 某某某。"** 以及更多文本来总结。

  这种格式提供了视觉锚点，有助于可读性和快速内容扫描。

  - 您可以跳过原始列表中的一些项目并重新编号。

  - 但是您不应该重新排序它们。

- 描述中允许额外的链接。这必须限制在一些罕见情况下。比如指向更大的概念、首字母缩略词定义或参考资料（书籍、传记等）。

## 编辑方针

每个列表的一般编辑方针在 [它们的介绍中有提示](https://github.com/kdeldycke/awesome-template#readme)。

还有一些根据列表的具体规则：

### [`awesome-engineering-team-management`](https://github.com/kdeldycke/awesome-engineering-team-management)：项目顺序

项目大致按以下顺序排列：

1. 首先我们会找到对软件开发人员或新经理有吸引力的内容。我们追求可访问性，针对更广泛的受众并提供温和的介绍。
1. 然后我们可以有几个真实的用例或轶事，这使主题更加实用和相关。
1. 第三，我们可能会添加几个参考资料来概括概念，提供系统化的解决方案并展示更广泛的思维框架。
1. 最后是最愤世嫉俗或最悲观的内容，这些内容作为警示故事或恶化条件的警告信号具有一定的效用。

### [`awesome-falsehood`](https://github.com/kdeldycke/awesome-falsehood)：候选项

在贡献之前，确保您想要添加的新链接是一个好的候选项。

这是一个非限制性的适合包含在 `awesome-falsehood` 列表中的项目列表。

#### 谬误文章

遵循 *谬误* 模式的文章是包含在这个精彩列表中的主要候选者。

这些文章从开发人员对领域有天真和简单看法的假设开始。然后继续列出程序员可能持有的一系列坦率假设。每一个都是故意错误的，在最佳形式下用反例说明。

谬误列表被精心设计为旨在完善概念的进展。阅读完整个谬误列表后，读者应该对领域有更好的概述，同时消除其神话，指出常见陷阱并展示其微妙之处。

*谬误* 文章在某种意义上是一套冗长的单元测试，涵盖了现实世界使用提供的广泛边缘情况。世界是混乱的。发现一个领域比预期复杂得多会导致挫折感。并导致掀桌子 `(╯°□°)╯︵ ┻━┻`。这是该列表的绝佳候选者的标志！

仅适用于一个产品（或服务）的文章不能被认为足够通用，应该避免。

#### 库

编程库或模块也是好的候选者，如果它们解决或减少了上述 *谬误* 文章指出的复杂性。

这样我们就可以把桌子放回原位。`┬─┬ ノ( ゜-゜ノ)`

#### 数据结构

足够通用以涵盖和解决大多数谬误的数据模型和结构也欢迎在此页面中出现。

## 常见问题

一些案例来说明策展过程。

### 我可以重写您的句子和段落吗？

可以。我不是母语使用者，所以我的一些写作可能有点花哨。如果您可以提出我初始文本的更短、更直接、更准确的版本，请继续！这些改进 [为两种读者都增加了很多可读性](https://github.com/kdeldycke/awesome-falsehood/pull/105)。

### 我可以为列表提议 YouTube 视频吗？

可以，但尝试将视频的开始精确定位到相关时间。比如在 YouTube URL 中使用 `&t=13m30s` 参数。

比视频更好的是：有其书面转录的链接。或者演示幻灯片，如果它没有稀释要表达的观点。

### 我可以链接到 X 帖子吗？

可以，但首先尝试在作者制作的内容中搜索：有时该作者将其咆哮编辑成其他地方更易于消化的文章。我们会更喜欢链接到那个。

### 如何防止链接腐烂？

[正如贡献者指出的](https://github.com/kdeldycke/awesome-engineering-team-management/issues/52#issue-1499417056)：

> 这里的链接有下线的趋势。为了使这成为长期价值的资源，可以通过存档页面来避免链接腐烂。

这是真的。

如果原始 URL 不再可访问，我不介意用替代的存档/缓存链接替换原始 URL。

损坏的链接令人沮丧。我们会逐一修复它们。有些链接已被移动到新域名，有些则完全消失了，我们将用[存档链接](#url)来替代它们。

如果您发现损坏的链接，请提出 PR 来修复它。或者只是将其报告为问题，我会完成这项工作。

### 您将如何存档下线的文章？

这个问题指出了我们需要在它们下线 *之前* 存档它们的悖论。

没有必要抢先存档内容。存在其他人这样做的激励：

- 这个列表足够受欢迎，其内容被常规存档爬虫收集。
- 这个列表中的热门内容自然被重视它们的用户存档。
- 关心自己内容或从这个列表提供的 SEO 价值中受益的作者有动机保持它们在原始 URL 可用。

尽管有这些激励措施，内容仍有可能完全从网络上消失，且没有[存档副本](#url)。这也不是世界末日。也许这些内容本来就不值得保留，原本就不适合被收录。可以把这种极端情况看作是内容的自然选择过程，有助于实现自然的内容筛选和整理。

### 为什么删除不活跃的 GitHub 项目？

未维护的 GitHub 仓库通常 [被其所有者存档](https://docs.github.com/en/repositories/archiving-a-github-repository/archiving-repositories)。但有些是事实上未维护的，或者被其作者原样遗弃，没有明确存档。

无论哪种方式，如果它们所处理的空间很拥挤，并且列表中引用了其他仓库，则该链接是删除以减少噪音的好候选者。

另一方面，如果项目已经在其他地方被分叉或重启，我们现在可以指出新位置。

### 为什么我的商业项目不在列表中？

可能是因为核心内容在付费墙后面。特别是如果有更好的在线资源，它们更广泛，可以免费访问。

这对 SaaS 和其他许可软件尤其如此。如果有开源项目可用，我们宁愿指向那个而不是商业解决方案。

这些替代方案不需要更好。如果它们足够好以从中获得灵感或开始没有进入障碍的事情，它们就符合条件。

因此，对于一组多个重叠的项目，我们会将商业项目视为重复项并删除它们，以保持列表精简。

### 为什么我的链接被拒绝了？

如果您的链接被拒绝，必须有动机并作为对您 PR 的评论向贡献者解释。

拒绝的一些原因，通常重叠，包括：

- 内容重复
- 缺乏原创性
- 现有内容的简单重复
- 没有说明新链接对现有资料库有什么新增价值
- 所在部分内容过于拥挤，[需要的是更好的整理而非添加更多内容](https://github.com/kdeldycke/awesome-iam/pull/76)
- [不够通用，或过于特定于某一产品或公司](https://github.com/kdeldycke/awesome-falsehood/pull/31#issuecomment-407667679)
- 带有营销性质的内容，仅为提升 SEO 而添加
- [已经有太多链接指向同一个商业域名](https://github.com/kdeldycke/awesome-iam/pull/179#issuecomment-3023031941) （两个链接就足够了）
- 对提出的问题缺乏反馈
- 偏离了本贡献指南的要求
- 违反了[行为准则](code-of-conduct.md)

### 我如何强制将链接加入列表？

如果您的贡献被拒绝，有一种方法可以绕过策展规则。您可以 [购买赞助](https://github.com/sponsors/kdeldycke) 并在此仓库的顶部拥有您的产品、徽标和链接！🤗 就像 [Descope 在 awesome IAM 列表上做了一年](https://twitter.com/kdeldycke/status/1676963147104784386)。

## [`awesome-falsehood`](https://github.com/kdeldycke/awesome-falsehood) 的常见问题

这些问题专门针对 [Awesome Falsehood](https://github.com/kdeldycke/awesome-falsehood) 项目。

### 为什么不在列表中复制谬误？

在仓库中编译所有谬误可能是个好主意。它将允许社区维护和丰富它们。它还可以提高整体质量，因为大多数外部文章不努力说明或解释为什么谬误是谬误。

但这是一个很大的努力，为了保持简单，我们只是在这个列表中收集外部文章。与此同时，如果您想添加谬误，我会要求潜在贡献者 [在其他地方托管它们](https://github.com/kdeldycke/awesome-falsehood/issues/46)。

此外，如果我们必须在此仓库中托管原始谬误，我们可能必须 [检查许可证并寻求原作者的许可](https://github.com/kdeldycke/awesome-falsehood/issues/24#issuecomment-354112401)。
