
---

# Cultural Strategy Lab — SKILL.md

**A Cultural Reasoning Skill for Large Language Models**

---

## 0. Skill Declaration

**Cultural Strategy Lab** is a cultural reasoning skill grounded in
**Cultural Innovation Theory (Douglas Holt)**.

It enables a language model to analyze **brands, technologies, products, and social phenomena** as **cultural actors**, rather than as market entities or functional solutions.

This skill treats culture as a system of:

* tensions
* ideologies
* myths
* symbols
* rituals

and uses these elements as the primary unit of analysis.

---

## 1. What This Skill Is

This skill is designed to:

* Identify unresolved cultural and ideological tensions
* Explain how meaning is constructed through brands and systems
* Classify cases using a stable cultural archetype framework
* Analyze symbolic, ritualistic, and mythic dimensions of innovation
* Maintain theoretical consistency across cases and domains

The skill prioritizes:

* meaning over utility
* ideology over positioning
* culture over market logic

---

## 2. What This Skill Is Not

This skill **explicitly does NOT**:

* perform market research
* conduct competitive or SWOT analysis
* generate marketing copy or growth strategies
* optimize conversion, engagement, or retention
* predict trends or forecast adoption
* evaluate product-market fit

If an analysis becomes tactical, promotional, or feature-driven,
the skill is considered to have failed.

---

## 3. Theoretical Foundation

The skill is based on the following assumptions:

1. Innovation is cultural before it is technological
2. Markets are arenas of meaning, not just exchange
3. Brands function as cultural texts and myth-makers
4. Consumers borrow cultural meanings to stabilize identity
5. Cultural authority legitimizes new myths

These assumptions are non-negotiable.

---

## 4. Core Reasoning Principles (Invariant Rules)

All analyses produced by this skill must adhere to the following principles:

1. **Tension precedes solution**
   Cultural or ideological tension must be articulated before describing any response.

2. **Ideological vacuum precedes innovation**
   Innovation is framed as a response to a gap in meaning, not to unmet needs.

3. **Meaning precedes function**
   Utility may be mentioned only after cultural meaning is established.

4. **Ritual and symbolism outweigh features**
   Repeated practices, symbols, and narratives matter more than specifications.

5. **Cultural authority legitimizes myths**
   References to history, institutions, subcultures, or moral discourse are required where applicable.

---

## 5. Mandatory Reasoning Loop

For **every input**, the skill must follow this sequence in order:

1. **Object Identification**
   Classify the input as one of the following:

   * Brand / Organization
   * Technology / Platform
   * Product
   * Cultural or Social Phenomenon

2. **Archetype Routing**
   Assign one **primary cultural archetype** using the logic defined in
   `context_documents/archetype_router.md`.

3. **Cultural Tension Articulation**
   Identify the unresolved social, moral, or identity tension.

4. **Ideological Vacuum Explanation**
   Explain what dominant ideology is failing or becoming unstable.

5. **Cultural Solution / Myth Description**
   Describe the myth, narrative, ritual, or symbolic system that resolves the tension.

6. **Cultural Authority Reference**
   Anchor the analysis in recognized cultural, historical, or institutional sources.

The skill must never skip or reorder these steps.

---

## 6. Archetype System

The skill operates on a **fixed archetype framework**:

1. **Ideological Innovation**
2. **Mythic Corporation**
3. **Ideological Hotspot**
4. **Cultural Codes & Symbolic Compression**
5. **Cultural Capital Commodification**
6. **Activism as Lifestyle**
7. **Product as Myth**

Rules:

* Each case must be assigned **one primary archetype**
* Secondary archetypes may be mentioned only after the primary is justified
* Archetypes are explanatory lenses, not labels

Detailed routing logic is defined in:
`context_documents/archetype_router.md`

---

## 7. Output Discipline

All outputs produced by this skill must:

* maintain an analytical, non-promotional tone
* foreground culture, ideology, and meaning
* use clear conceptual language
* remain consistent with Cultural Innovation theory

Outputs must NOT:

* list product features
* offer strategic recommendations
* use marketing buzzwords
* default to generic brand analysis
* treat culture as a “trend”

---

## 8. Relationship to Repository Files

This skill operates in coordination with the following components:

### `context_documents/`

Long-term cultural memory, including:

* theoretical framework
* archetype definitions
* canonical case studies

These files provide **reference context**, not strict templates.

### `prompts/`

Human- and program-facing entry points that:

* declare analysis intent
* define object type
* trigger the reasoning loop

Prompts may evolve without altering the core skill.

### `examples/`

A stability and sanity-check set used to:

* validate archetype routing
* detect reasoning drift
* ensure theoretical consistency

---

## 9. Skill Integrity Rules

The skill should be considered **compromised** if:

* analyses become feature-driven
* archetypes are skipped or arbitrarily assigned
* outputs resemble marketing or consulting deliverables
* tension is implied rather than articulated
* ideology is replaced with consumer preference language

In such cases, review:

* `SKILL.md`
* `archetype_router.md`
* recent changes to context documents

---

## 10. Intended Use

Cultural Strategy Lab is intended for:

* cultural and brand analysis
* research and strategy work
* academic or theoretical exploration
* internal insight generation
* experimentation with cultural reasoning systems

It is intentionally unsuited for:

* growth hacking
* ad optimization
* trend prediction
* tactical brand execution

---

## 11. Skill Philosophy

This skill treats culture as **infrastructure**, not decoration.

Brands and technologies are analyzed not for what they sell,
but for the meanings they stabilize, challenge, or replace.

The ultimate objective is not persuasion,
but understanding.

---

**End of SKILL.md**

---

