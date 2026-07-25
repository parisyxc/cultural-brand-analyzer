
---

# Installing Cultural Strategy Lab into Claude (User Guide)

This guide explains how to install and use **Cultural Strategy Lab** as a local skill inside **Claude Code / Claude Desktop**.

No API key is required.

---

## Step 1. Download the Skill from GitHub

Clone or download the repository:

```bash
git clone https://github.com/parisyxc/skills.git
```

Navigate to the Cultural Strategy Lab directory:

```bash
cd skills/Cultural-Strategy-Lab
```

---

## Step 2. Install the Skill into Claude

Claude uses a local directory to store skills.

Copy the entire `Cultural-Strategy-Lab` folder into your Claude skills directory:

```bash
mkdir -p ~/.claude/skills
cp -r Cultural-Strategy-Lab ~/.claude/skills/
```

After copying, your directory structure should look like this:

```bash
~/.claude/skills/
└── Cultural-Strategy-Lab/
    ├── SKILL.md
    ├── ACTIVATE.md
    ├── DEACTIVATE.md
    ├── context_documents/
    ├── examples/
    ├── prompts/
    └── README.md
```

This completes the installation.

---

## Step 3. Start Claude

Launch Claude from your terminal:

```bash
claude
```

Or open Claude Desktop.

---

## Step 4. Activate the Skill (Required)

Claude does not automatically load skills.
You must activate the skill at the beginning of a session.

Copy and paste the following into Claude:

```text
Use the Cultural Strategy Lab skill.
Strictly follow the reasoning rules defined in SKILL.md.
Treat context_documents/ as long-term cultural reference.
Analyze all inputs through cultural tension,
ideological vacuum, and archetype logic.
Do NOT provide market analysis or tactical advice.
```

(You can also copy this directly from `ACTIVATE.md`.)

---

## Step 5. Run an Analysis

Once activated, you can analyze any case:

```text
Analyze Patagonia using Cultural Strategy Lab.
Identify the cultural tension, ideological vacuum,
and dominant archetype.
```

You may analyze:

* Brands
* Technologies
* Products
* Cultural or social phenomena

---

## Step 6. Verify Installation (Recommended)

To confirm the skill is working correctly:

1. Open `examples/01_brand_nike.md`
2. Copy the prompt under **How to Run (No API)**
3. Paste it into Claude

Correct behavior includes:

* Cultural tension appears before solutions
* Archetypes are explicitly named
* Minimal focus on features or tactics

---

## Step 7. Deactivate the Skill (Optional)

When you want to return to default Claude behavior, paste:

```text
Deactivate Cultural Strategy Lab skill and return to default Claude behavior.
```

(Available in `DEACTIVATE.md`.)

---

## Common Questions

### Does this require an API key?

No. This skill works entirely through local context and prompt control.

### Is this a Claude plugin?

No. Claude currently does not support user-installed plugins.
This skill operates as a **local cognitive framework**.

### Will Claude always remember the skill?

No. You must activate it in each new session.

---

## Summary

Installing Cultural Strategy Lab means:

* Copying it into `~/.claude/skills/`
* Activating it explicitly at session start
* Using it as a cultural reasoning framework

Once installed, it behaves like a reusable cognitive skill inside Claude.

---

## Final Note

Cultural Strategy Lab is not a tool.
It is a way of thinking.

Use it accordingly.

---

