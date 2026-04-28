# Prompt Generating

这是一个用于沉淀和管理提示词方法论与模板的仓库，重点服务于“把原始内容整理成结构化输出”的场景。

目前仓库已包含两份核心 skill：

- `skills/prompt-writing-skill.md`
- `skills/visual-summary-poster-skill.md`

其中，`prompt-writing-skill.md` 聚焦提示词写作方法论；`visual-summary-poster-skill.md` 聚焦把长文本、访谈稿、演讲稿、课程内容、教程说明转化为图片版图文海报。

---

## 仓库目标

这个仓库主要用于：

1. 沉淀高质量提示词写法
2. 抽象通用的提示词方法论
3. 为不同业务场景生成稳定、可复用的模板
4. 支持前端展示与后端解析友好的输出设计
5. 逐步形成可复用的 prompt skill 库
6. 支持从文本到图文海报的自动化生成流程

---

## 当前内容

### 1. Prompt Writing Skill

文件路径：

- `skills/prompt-writing-skill.md`

主要内容包括：

- 如何写任务定义
- 如何写基本要求
- 如何写提取重点
- 如何设计输出结构
- 如何让输出既便于阅读又便于解析
- 如何设计会议纪要类提示词
- 如何处理用户手动笔记、marker、高亮信息
- 如何设计待办事项和引用来源
- 如何避免流水账式输出

### 2. 图文海报生成 Skill

文件路径：

- `skills/visual-summary-poster-skill.md`

主要内容包括：

- 如何把原文提炼成图文海报结构
- 如何选择长图文或封面图
- 如何按内容类型自动匹配视觉风格
- 如何设计 8 种图文风格
- 如何把 HTML 中间页渲染成 PNG 图片
- 如何固定底部署名为“内容由嗒嗒AI生成”

目前内置 8 种风格：

1. 咨询卡片方法论风
2. 杂志深浅拼接风
3. 手账教程图解风
4. 极简金句分镜风
5. 小红书爆款笔记风
6. 奢华自然意境风
7. 软萌知识卡片风
8. 黑板报讲解风

---

## 方法论核心

### Prompt Writing Skill

这套方法的核心是把“原始内容整理类任务”统一拆成四段：

1. `任务定义`
2. `基本要求`
3. `提取重点`
4. `输出要求`

再结合以下原则提高输出质量：

- 先结果，后过程
- 先重点，后细节
- 按主题归纳，而不是按顺序复述
- 对核心数据与关键时间节点进行高亮
- 对用户手动标注内容提高权重
- 让输出既适合人读，也适合系统解析

### 图文海报生成 Skill

这套方法的核心是把“长文本转图文”拆成五步：

1. 理解原文主线
2. 抽象一级模块
3. 提炼卡片内容
4. 匹配视觉风格
5. 生成 HTML 并渲染为 PNG 图片

它强调：

- 不按原文段落机械切分
- 不堆砌所有信息
- 把同一逻辑层级的内容合并
- 根据内容类型选择视觉风格
- 最终输出图片，而不是 HTML

---

## 适用场景

目前这套方法特别适合以下类型任务：

- 会议纪要
- 访谈整理
- 课堂笔记
- 培训总结
- 医疗记录
- 销售沟通
- 面试分析
- 项目复盘
- 用户研究
- 商业增长复盘
- 教程图解
- 工具说明
- 课程长图
- 小红书风格图文
- 封面图生成

未来可以继续扩展到：

- 文档命名
- 文件归档
- 长文本压缩总结
- 主题抽取
- 决策信息抽取
- 自动待办抽取
- 多图轮播生成
- 视频封面生成

---

## 推荐使用方式

### 方式一：先用 skill，再生成具体 prompt

适合你先明确场景，再基于方法论产出专项提示词。

例如：

- 先参考 `prompt-writing-skill.md`
- 再生成“会议纪要提示词”
- 再生成“课堂笔记提示词”
- 再生成“销售复盘提示词”

### 方式二：把 skill 当作评审标准

当你写出一版 prompt 后，可以用这份 skill 检查：

- 任务定义是否清晰
- 基本要求是否抓住重点
- 提取重点是否覆盖完整链路
- 输出结构是否适合阅读和解析
- 是否避免了流水账输出

### 方式三：用图文海报生成 Skill 直接出图

适合把一段长文本直接转成图片版图文海报。

示例：

```text
请使用图文海报生成 Skill，把下面原文生成图片版图文海报。
风格：风格一，咨询卡片方法论风
输出形态：长图文
原文：
……
```

也可以让系统自动选择风格：

```text
请使用图文海报生成 Skill，把下面原文生成图片版图文海报。
风格：自动选择
输出形态：封面图
原文：
……
```

---

## 后续扩展建议

建议后续在仓库中逐步增加：

- `skills/meeting-minutes-skill.md`
- `skills/learning-notes-skill.md`
- `skills/interview-analysis-skill.md`
- `skills/sales-summary-skill.md`
- `templates/` 目录下的专项 prompt 模板
- `examples/` 目录下的输入输出示例
- `examples/visual-summary/` 目录下的图文海报示例

推荐目录结构：

```text
Prompt_Generating/
├── README.md
├── skills/
│   ├── prompt-writing-skill.md
│   ├── visual-summary-poster-skill.md
│   ├── meeting-minutes-skill.md
│   └── ...
├── templates/
│   ├── meeting-minutes-template.md
│   ├── class-notes-template.md
│   └── ...
└── examples/
    ├── meeting-example.md
    └── visual-summary/
        ├── cover-example.md
        └── long-poster-example.md
```

---

## 一句话总结

这个仓库的目标，不是存零散 prompt，而是沉淀一套能稳定生成高质量结构化内容与图文海报的 prompt skill 系统。
