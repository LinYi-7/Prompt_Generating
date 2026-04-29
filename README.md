# Prompt Generating

这是一个用于沉淀和管理提示词方法论与模板的仓库，重点服务于“把原始内容整理成结构化输出”的场景。

目前仓库已包含一份核心 skill：

- `skills/prompt-writing-skill.md`

这份 skill 不是单一模板，而是一套可复用的提示词写作方法论，适合持续扩展到会议纪要、课堂笔记、访谈整理、销售沟通、医疗记录、项目复盘等多个场景。

---

## 仓库目标

这个仓库主要用于：

1. 沉淀高质量提示词写法
2. 抽象通用的提示词方法论
3. 为不同业务场景生成稳定、可复用的模板
4. 支持前端展示与后端解析友好的输出设计
5. 逐步形成可复用的 prompt skill 库

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

---

## 方法论核心

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

未来可以继续扩展到：

- 文档命名
- 文件归档
- 长文本压缩总结
- 主题抽取
- 决策信息抽取
- 自动待办抽取

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

---

## 后续扩展建议

建议后续在仓库中逐步增加：

- `skills/meeting-minutes-skill.md`
- `skills/learning-notes-skill.md`
- `skills/interview-analysis-skill.md`
- `skills/sales-summary-skill.md`
- `templates/` 目录下的专项 prompt 模板
- `examples/` 目录下的输入输出示例

推荐目录结构：

```text
Prompt_Generating/
├── README.md
├── skills/
│   ├── prompt-writing-skill.md
│   ├── meeting-minutes-skill.md
│   └── ...
├── templates/
│   ├── meeting-minutes-template.md
│   ├── class-notes-template.md
│   └── ...
└── examples/
    ├── meeting-example.md
    └── ...
```

---

## 一句话总结

这个仓库的目标，不是存零散 prompt，而是沉淀一套能稳定生成高质量 prompt 的方法论，并逐步形成可复用的 prompt skill 系统。
