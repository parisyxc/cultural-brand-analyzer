# Cultural Archetype Test Guide

This document summarizes the validation tests
for each cultural innovation archetype used in the project.

Its purpose is to verify whether archetype routing
and case internalization are functioning correctly
inside the Claude Skill.

This is a project note, not an analytical framework.

---

## How to Use This Document

After adding or modifying:
- Archetype cases
- Context documents
- System prompts

Run the corresponding test prompts below.

If Claude responds in the expected way,
the archetype is correctly internalized.

If not, review:
- case_*.md structure
- archetype_router.md routing logic
- system prompt constraints

---

## Archetype 1: Ideological Innovation
**Reference Case: Nike**

### Test Prompt
> Analyze a new fitness or productivity brand using cultural innovation theory.

### Expected Signals
- Focus on identity, dignity, or moral reframing
- Discussion of struggle, effort, or self-worth
- Minimal attention to features or market gaps

### Failure Mode
- Overemphasis on differentiation or positioning
- Treating innovation as functional improvement

---

## Archetype 2: Mythic Corporation
**Reference Case: Jack Daniel's**

### Test Prompt
> Analyze a traditional craft or heritage brand using cultural innovation theory.

### Expected Signals
- Emphasis on origin, founder myth, and restraint
- Organization treated as the source of meaning
- Minimal reference to marketing communication

### Failure Mode
- Focus on storytelling campaigns
- Treating authenticity as a branding tactic

---

## Archetype 3: Ideological Hotspot
**Reference Case: Ben & Jerry's**

### Test Prompt
> Analyze a socially driven brand or activist startup using cultural innovation theory.

### Expected Signals
- Brand framed as a moral or political actor
- Explicit discussion of values, stances, and social debate
- Recognition of ideological conflict

### Failure Mode
- Framing the case as CSR or ESG optimization
- Treating activism as reputation management

---

## Archetype 4: Cultural Codes & Symbolic Compression
**Reference Case: Marlboro**

### Test Prompt
> Analyze a lifestyle brand that relies heavily on visual identity.

### Expected Signals
- Focus on symbols, repetition, and archetypes
- Explanation of meaning through encoding, not narrative
- Recognition of instant identity signaling

### Failure Mode
- Over-analysis of brand story or messaging
- Treating symbols as decorative rather than functional

---

## Archetype 5: Cultural Capital Commodification
**Reference Case: Starbucks**

### Test Prompt
> Analyze a service or lifestyle brand using cultural innovation theory.

### Expected Signals
- Discussion of taste, ritual, and cultural learning
- Consumption framed as self-upgrading
- Emphasis on language, behavior, and space

### Failure Mode
- Treating experience as UX optimization
- Reducing ritual to convenience or habit formation

---

## Archetype 6: Activism as Lifestyle
**Reference Case: Patagonia**

### Test Prompt
> Analyze a sustainability-focused or mission-driven brand.

### Expected Signals
- Values embedded in behavior and operations
- Emphasis on durability, restraint, and long-term practice
- Activism framed as identity, not messaging

### Failure Mode
- Framing the case as green marketing
- Overreliance on stated mission or slogans

---

## Archetype 7: Product as Myth
**Reference Case: Vitaminwater**

### Test Prompt
> Analyze a consumer product positioned as healthier, smarter, or more responsible.

### Expected Signals
- Product experienced as a symbolic solution
- Design and ritual outweigh functional superiority
- Consumption framed as a completed moral act

### Failure Mode
- Overemphasis on ingredients or performance
- Treating symbolism as secondary decoration

---

## Cross-Archetype Sanity Check

When testing any archetype, verify that:

- Claude routes the case before deep analysis
- One archetype is dominant
- Secondary influences are noted but not merged
- Cultural tension precedes solution

If these conditions are met,
the cultural reasoning engine is functioning as intended.

---

## Maintenance Notes

- Update this document whenever a new archetype is added
- Re-run tests after modifying system prompt or context documents
- Use failures as diagnostic signals, not errors

Correct routing enables correct thinking.
