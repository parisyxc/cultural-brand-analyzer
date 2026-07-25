
---

# Getting Started（本地使用 · 无需 API）

Cultural Strategy Lab **不要求你调用任何 API 才能使用**。

这是一个**文化推理 Skill（Cognitive Skill）**，核心价值在于：

* `SKILL.md`：文化推理规则（Skill Contract）
* `context_documents/`：长期文化知识与案例
* `prompts/`：可复用的分析入口
* `examples/`：验证推理是否稳定的参考集
* `ACTIVATE.md`：快速激活使用Cultural Strategy Lab
* `DEACTIVATE.md`：快速退出使用Cultural Strategy Lab

你可以把它当作一个**可被 Claude / 任何 LLM 加载的文化思维系统**。

---

## 1. 本地使用方式（推荐）

### 方式 A：作为 Claude Code / Claude Desktop 的本地 Skill

这是**最推荐的使用方式**，不涉及任何 API。

#### Step 1：放置 Skill

将整个项目放入：

```bash
~/.claude/skills/Cultural-Strategy-Lab/
```

结构示例：

```bash
.claude/skills/Cultural-Strategy-Lab/
├─ SKILL.md
├─ context_documents/
├─ prompts/
├─ examples/
└─ README.md
```

#### Step 2：在 Claude Code 中使用

在 Claude Code / Claude Desktop 中：

1. 打开任意项目或空白会话
2. 明确告诉 Claude：

> 请使用 `Cultural Strategy Lab` Skill
> 并遵循 `SKILL.md` 中的推理规则
> 结合 `context_documents/` 进行分析

3. 然后输入你的分析请求，例如：

> Analyze Patagonia using cultural innovation theory.

📌 **此方式完全不需要 API key，也不会产生费用**
📌 Claude 会把这套 Skill 当作“长期上下文 + 推理约束”

---

## 2. 使用 prompts 进行结构化分析（无代码）

如果你希望**每次分析都有稳定结构**，可以直接使用 `prompts/` 目录中的文件。

例如：

```text
prompts/analyze_brand.txt
```

你可以在 Claude 中这样说：

> 使用 analyze_brand 的结构，
> 按 Cultural Strategy Lab 的方法分析 Patagonia。

这适合：

* 咨询 / 研究场景
* 写分析报告
* 做文化洞察练习

---

## 3. 使用 examples 作为参考与自检

`examples/` 不是 demo，而是**推理稳定性验证集**。

你可以：

* 先阅读 examples
* 再对照 Claude 的输出
* 判断是否出现：

  * feature 化
  * 市场化
  * archetype 跑偏

如果输出和 examples 的逻辑一致，说明 Skill 正常工作。

---

## 4. 关于 API（可选，而非必需）

> **你不需要 API 才能使用 Cultural Strategy Lab。**

项目中提供的 `api/` 目录仅用于：

* 研究型自动化
* 批量分析
* 工程集成

如果你只是：

* 做文化分析
* 写研究
* 思考品牌与社会

👉 **完全可以忽略 `api/` 目录。**

---

## 5. 推荐的使用心法（非常重要）

在使用本 Skill 时，请记住：

* 不要问“这个品牌做得好不好”
* 而是问“它在解决什么文化矛盾”
* 不要急着要结论
* 而是允许 tension 先展开

这是一个**思考工具，而不是答案生成器**。

---

## 6. 最小使用示例（纯自然语言）

你可以直接对 Claude 说：

> 使用 Cultural Strategy Lab，
> 从文化矛盾、意识形态真空和神话结构三个层面，
> 分析 Patagonia。

或者：

> 用文化创新理论分析 Quiet Quitting，
> 并判断它最接近哪一种文化原型。

---

## 总结一句话

> **Cultural Strategy Lab 首先是一个“文化思维系统”，
> 其次才是一个可调用的程序。**

你可以：

* 只用 Markdown + Claude
* 不写一行代码
* 不花一分钱
* 但仍然完整使用这个 Skill

---


