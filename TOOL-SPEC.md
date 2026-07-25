# Cultural Brand Analyzer — Tool Spec

> 轻封装：把 `cultural-brand-pool`（= Cultural Strategy Lab，Douglas Holt 文化创新理论）从"分析技能"框成一个 **input → output 的工具**。
> 引擎不变（`SKILL.md` 6 步推理环 + 7 个固定原型 + `prompts/` + `context_documents/` 案例库）。改的是外壳、命名、I/O 契约。
> 定位：tool-led（帮你想清楚品牌的文化意义，直接给分析），不是卖咨询过程。

---

## 1 · 是什么（一句话）

**Cultural Brand Analyzer** —— 输入一个品牌 / 产品 / 技术 / 社会现象，输出一份**文化分析**：它属于哪个文化原型、化解了什么文化张力、哪种主导意识形态正在失效、以及它用什么神话/符号/仪式来回应。基于 Holt 文化创新理论。

## 2 · Input → Output 契约

**INPUT（用户提供）**
- `subject` —— 要分析的对象：一个品牌 / 组织 / 技术 / 产品 / 社会现象
- （可选）`context` —— 它是什么、品类、背景

**OUTPUT（工具产出的分析，严格按 6 步推理环）**
1. **Object type** —— 对象归类（品牌·组织 / 技术·平台 / 产品 / 文化·社会现象）
2. **Primary archetype** —— 一个主文化原型（7 选 1，见下）
3. **Cultural tension** —— 未解的社会 / 道德 / 身份张力
4. **Ideological vacuum** —— 哪种主导意识形态正在失效或松动
5. **Cultural solution / myth** —— 化解张力的神话 + 符号 + 仪式
6. **Cultural authority** —— 分析锚定的文化 / 历史 / 制度来源

> 一句话：**输入一个文化行动者,拿一份结构化的文化战略分析。**

**7 个固定原型**：Ideological Innovation · Mythic Corporation · Ideological Hotspot · Cultural Codes & Symbolic Compression · Cultural Capital Commodification · Activism as Lifestyle · Product as Myth。每个 case 只赋 **1 个主原型**;次原型须先论证主原型后才提。

## 3 · 这个工具的性质（和 GEO 的关键区别）

| | **GEO Content Planner** | **Cultural Brand Analyzer** |
|---|---|---|
| 输出类型 | 可执行的**内容计划**（query/AU/分发） | 一份**文化分析 / 战略透镜**（不是可发布物料） |
| 有没有运营层 | 有（月度追踪 recurring） | **无** —— 一次性分析工具（one-shot） |
| 帮你 | **做**（产出成品） | **想清楚**（给意义/立场的判断） |

所以它是 tool-led 里"**帮你想**"那一类的旗舰;上游给定位/内容一个"文化立场"的地基。

## 4 · 纪律必须保留（这是它的价值,不能稀释）

工具**明确不做**：市场调研 · SWOT · 定位文案 · 增长/转化建议 · 趋势预测。
> 一旦分析变成战术、推销、或功能罗列，这个技能就算失败。

在极简/tool-led 的呈现里也要守住这条——**卖的是"文化意义的判断",不是"营销建议"**。把这条写进产品页,反而是差异化(别的工具做不到这种克制)。

## 5 · 命名与结构

- **公开工具名**：`Cultural Brand Analyzer`（按成果命名）。
- **引擎**：`cultural-brand-pool/`（SKILL + prompts + archetype_router + context 案例库）保留为底层。
- **案例库 = examples/**（Nike / Peloton / Notion / TikTok / quiet quitting / digital nomad）——天生公开的 worked-example（capability demo,非客户工作),正是网站要的公开证据。
- **公开 demo**：用**公开品牌**跑一份分析当 demo case（见 `cultural-brand-analyzer-demo.html`,用 Liquid Death）——文化分析是解读性的,用真实公开品牌更可信,且不涉及客户工作。

## 6 · 与轻量化目标的关系

- 呈现从"痛点→为什么→如何服务→Book a call" → **"工具名 → 一句它做什么 → input → output → demo case → 用它"**。
- 输出是分析,所以 demo 直接展示"输入一个品牌 → 拿到 6 段文化分析"。
- 与 GEO 同为 tool-led 主角,但一个"帮你做"、一个"帮你想";两者互补。

## 7 · 待办（如果采纳）

1. registry：`cultural-brand-analyzer`（general/tool，S2），指向本 spec + demo；examples/ 作为公开案例库。
2. 网站：用 `cultural-brand-analyzer-demo.html` 的样式做第二个"极简 tool + demo"卡片。
3. 其余成熟 use-case（短视频生产、小红书趋势）复制同一结构。
