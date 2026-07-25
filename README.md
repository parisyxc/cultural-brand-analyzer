# Cultural Brand Analyzer

> Read a brand's meaning, not its tactics. Grounded in Douglas Holt's Cultural Innovation Theory.

Give it a brand, product, technology, or social phenomenon, and it returns a **cultural analysis**: the archetype it belongs to, the cultural tension it resolves, the ideology failing around it, and the myth, symbols, and rituals it uses.

## Input → Output

**Input** — `subject` (a brand / product / technology / phenomenon) + optional `context`.

**Output** — a structured analysis in a fixed 6‑step reasoning loop:

1. **Object type** — brand / technology / product / phenomenon
2. **Primary archetype** — one of 7 (see below)
3. **Cultural tension** — the unresolved social / moral / identity tension
4. **Ideological vacuum** — which dominant ideology is failing or loosening
5. **Cultural solution / myth** — the myth + symbols + rituals that resolve the tension
6. **Cultural authority** — the cultural / historical source the analysis anchors to

**7 archetypes:** Ideological Innovation · Mythic Corporation · Ideological Hotspot · Cultural Codes & Symbolic Compression · Cultural Capital Commodification · Activism as Lifestyle · Product as Myth.

## Deliberately *not*

Market research · SWOT · positioning copy · growth recommendations. It reads meaning, not tactics — that restraint is the point.

## What's in this repo

| Path | What it is |
|------|-----------|
| `SKILL.md` | The cultural reasoning rules (the skill contract) |
| `TOOL-SPEC.md` | The input → output contract and how it's framed as a tool |
| `context_documents/` | Long‑term cultural knowledge + worked cases (Nike, Patagonia, Marlboro, Ben & Jerry's, …) |
| `prompts/` | Reusable analysis entry points |
| `examples/` | A reasoning‑stability reference set (public brands & phenomena) |
| `case_study/` | **Full worked analyses on public brands** — Smythson (Mythic Corporation) · Rapha (Cultural Capital Commodification), plus a documented archetype‑routing decision |
| `demo/cultural-brand-analyzer-demo.html` | A worked analysis on a public brand (Liquid Death) |
| `ACTIVATE.md` / `DEACTIVATE.md` | Quick load / unload of the skill |
| `USAGE.md` | Full local‑usage guide (no API required) |

## Use it

No API needed — see `USAGE.md`. Load it as a local skill in Claude, then ask it to analyze a subject using the reasoning rules in `SKILL.md` and the cases in `context_documents/`.

**On the examples and case studies:** every brand referenced in this repo is analyzed from public material only. These are interpretive cultural readings — capability demonstrations, not client work, and not claims about any company's internal strategy or results.

---

*Part of theAgenticMarketing — a marketing toolkit for founders, solo operators, and agency owners. Examples and demos use public brands only; no client work is included.*
