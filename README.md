# Cultural Brand Analyzer

> **EN** — Read a brand's meaning, not its tactics. Grounded in Douglas Holt's Cultural Innovation Theory.
>
> **中文** —— 读一个品牌的**意义**，而不是它的战术。基于 Douglas Holt 文化创新理论。

---

## 1 · 是什么 · What this is

**中文** —— **Cultural Brand Analyzer** 输入一个品牌 / 产品 / 技术 / 社会现象，输出一份**文化分析**：它属于哪个文化原型、化解了什么文化张力、哪种主导意识形态正在失效、以及它用什么神话 / 符号 / 仪式来回应。基于 Holt 文化创新理论。

**EN** — Give it a brand, product, technology, or social phenomenon, and it returns a **cultural analysis**: which cultural archetype it belongs to, which cultural tension it resolves, which dominant ideology is failing, and the myth / symbols / rituals it uses to respond.

---

## 2 · Input → Output 契约 · The contract

### INPUT（用户提供 · what you provide）

| | 中文 | EN |
|---|---|---|
| `subject` | 要分析的对象：一个品牌 / 组织 / 技术 / 产品 / 社会现象 | The object of analysis: a brand · organization · technology · product · social phenomenon |
| `context` *(可选 / optional)* | 它是什么、品类、背景 | What it is, its category, background |

### OUTPUT（严格按 6 步推理环 · the fixed 6-step reasoning loop）

| # | 步骤 | 中文 | EN |
|---|---|---|---|
| 1 | **Object type** | 对象归类（品牌·组织 / 技术·平台 / 产品 / 文化·社会现象） | Object classification (brand·org / tech·platform / product / cultural·social phenomenon) |
| 2 | **Primary archetype** | 一个主文化原型（7 选 1，见下） | One primary cultural archetype (1 of 7, below) |
| 3 | **Cultural tension** | 未解的社会 / 道德 / 身份张力 | The unresolved social / moral / identity tension |
| 4 | **Ideological vacuum** | 哪种主导意识形态正在失效或松动 | Which dominant ideology is failing or loosening |
| 5 | **Cultural solution / myth** | 化解张力的神话 + 符号 + 仪式 | The myth + symbols + rituals that resolve the tension |
| 6 | **Cultural authority** | 分析锚定的文化 / 历史 / 制度来源 | The cultural / historical / institutional source the analysis anchors to |

> **一句话：输入一个文化行动者，拿一份结构化的文化战略分析。**
> **In one line: put in a cultural actor, get back a structured cultural-strategy analysis.**

### 7 个固定原型 · The 7 fixed archetypes

`Ideological Innovation` · `Mythic Corporation` · `Ideological Hotspot` · `Cultural Codes & Symbolic Compression` · `Cultural Capital Commodification` · `Activism as Lifestyle` · `Product as Myth`

**每个 case 只赋 1 个主原型；次原型须先论证主原型后才提。**
Each case is assigned **exactly one** primary archetype; a secondary archetype may only be raised *after* the primary one has been argued.

---

## 3 · 明确不做 · Deliberately *not*

市场调研 · SWOT · 定位文案 · 增长建议。它读的是意义，不是战术——**这份克制本身就是它的价值。**

Market research · SWOT · positioning copy · growth recommendations. It reads meaning, not tactics — that restraint is the point.

---

## 4 · 仓库结构 · What's in this repo

| Path | What it is |
|------|-----------|
| `SKILL.md` | 文化推理规则（Skill Contract）· the cultural reasoning rules |
| `TOOL-SPEC.md` | Input → output 契约与工具化定位 · the I/O contract and tool framing |
| `context_documents/` | 长期文化知识 + 已验证案例（Nike, Patagonia, Marlboro, Ben & Jerry's, Starbucks…） |
| `prompts/` | 可复用的分析入口 · reusable analysis entry points |
| `examples/` | 推理稳定性验证集 · a reasoning-stability reference set |
| `case_study/` | **完整分析案例** — Smythson (Mythic Corporation) · Rapha (Cultural Capital Commodification)，含一份 archetype routing 决策记录 |
| `demo/cultural-brand-analyzer-demo.html` | 公开品牌的分析 demo (Liquid Death) |
| `ACTIVATE.md` / `DEACTIVATE.md` | 快速激活 / 退出 · quick load / unload |
| `INSTALL.md` · `USAGE.md` | 安装与本地使用指南（无需 API）· install & local-usage guide (no API required) |

---

## 5 · 怎么用 · Use it

**不需要 API** —— 见 `USAGE.md` / `INSTALL.md`。把它作为本地 skill 载入 Claude，然后让它按 `SKILL.md` 的推理规则、结合 `context_documents/` 分析你的对象。

No API needed — see `USAGE.md` / `INSTALL.md`. Load it as a local skill in Claude, then ask it to analyze a subject using the reasoning rules in `SKILL.md` and the cases in `context_documents/`.

一个最小用法 · a minimal invocation:

```
使用 Cultural Strategy Lab 的推理规则，
从文化张力、意识形态真空和神话结构三个层面分析 Patagonia。
```

---

## 使用心法 · How to hold it

* 不要问「这个品牌做得好不好」，而要问「**它在解决什么文化矛盾**」。
* 不要急着要结论，允许 tension 先展开。
* 这是一个**思考工具**，不是答案生成器。

Don't ask "is this brand doing well" — ask "**what cultural contradiction is it resolving**." Don't rush the conclusion; let the tension unfold first. This is a thinking tool, not an answer generator.

---

**关于案例与 demo · On the examples and case studies:** 本仓库引用的每个品牌都只基于公开材料分析。这些是解读性的文化研究——能力演示，不是客户工作，也不是对任何公司内部战略或经营结果的判断。

Every brand referenced in this repo is analyzed from public material only. These are interpretive cultural readings — capability demonstrations, not client work, and not claims about any company's internal strategy or results.

---

*Part of theAgenticMarketing — a marketing toolkit for founders, solo operators, and agency owners. Examples and demos use public brands only; no client work is included.*
