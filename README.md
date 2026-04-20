# **Professor Synapse 🧙🏾‍♂️**

> **TL;DR** |
> ---
> Professor Synapse 🧙🏾‍♂️ is a wise AI guide that helps users achieve their goals by summoning expert agents perfectly suited to their tasks. It gathers context, aligns with user preferences, and creates specialized agents using a structured template to provide targeted expertise and step-by-step guidance.

## Introduction

**Professor Synapse 🧙🏾‍♂️** is a wise AI guide that helps users achieve their goals by summoning expert agents perfectly suited to their specific tasks. It gathers context about your goals, then creates and orchestrates specialized agents using a structured template to provide targeted expertise and actionable guidance.

---

## Two Ways to Use Professor Synapse

### 1. Universal Prompt (Any AI)

The classic approach — copy and paste the prompt into any AI chat interface.

**File:** `Prompt.md`

**Works with:** ChatGPT, Claude, Gemini, or any LLM that accepts system prompts.

**Setup:**
1. Open `Prompt.md` and copy the contents
2. Paste into your AI's system prompt or custom instructions
3. Start chatting!

### 2. Claude Skill (Draft-First)

A more powerful version designed for Claude. This skill is **draft-first by default** — it proposes expert agents in chat, asks before saving files, and treats persistence as an explicit maintenance action.

**Folder:** `professor-synapse/`

**Features:**
- 🔎 **Domain Researcher** agent that browses the web before drafting new experts
- 📝 **Draft-first expert creation** — new agents are proposed in chat before any save
- 🧠 **Pattern suggestions** — reusable learnings are proposed instead of auto-written
- 📋 **Auto-generated index** — agents are catalogued when explicitly rebuilt
- 🎭 **Multi-agent debates** — convene multiple specialists for complex decisions
- 🔄 **Smart updates** — fetch updates from GitHub without blindly overwriting customizations
- 🔧 **Optional packaging** — rebuild and package only when explicitly requested
- 🔒 **Safer defaults** — no automatic dependency installation or silent skill self-modification

---

## Claude Skill Setup

### Install

1. **Download** `professor-synapse.zip` from this repo

2. **Add to Claude:**
   - Open Claude → **Settings** → **Capabilities** → **Skills**
   - Click **Add new skill**
   - Upload `professor-synapse.zip`

3. **Start using it:**
   - Professor Synapse activates when you say things like:
     - "Help me with..."
     - "I need guidance on..."
     - "I need an expert for..."

### Skill Structure

```
professor-synapse/
├── SKILL.md                      # Main identity + workflow
├── agents/
│   ├── INDEX.md                  # Auto-generated registry
│   └── domain-researcher.md      # Base research agent
├── references/
│   ├── safety-protocol.md        # Safety defaults and trust boundaries
│   ├── agent-template.md         # Structure for new agents
│   ├── domain-expertise.md       # Domain mappings
│   ├── file-operations.md        # How to save/update files
│   ├── convener-protocol.md      # Multi-agent debate facilitation
│   ├── update-protocol.md        # GitHub update workflow
│   └── rebuild-protocol.md       # Local change rebuild workflow
└── scripts/
    ├── rebuild-index.sh           # Regenerate INDEX.md
    ├── fetch-github-file.sh       # Fetch files from GitHub
    └── github_blob_parser.py      # Parse GitHub HTML for content
```

### Recommended: Claude Project Setup

For the best experience, create a dedicated Claude project for working with Professor Synapse:

1. **Create a new project** in Claude Desktop
2. **Add these project instructions:**

```
Begin the conversation with "🧙🏿‍♂️: [acknowledgment of user request]. Conjuring my professor-synapse skill to assist you."

Then follow these instructions:
1. FIRST: Use the `view` tool to check /mnt/skills/user/ for the skill
2. Read the SKILL.md file for that skill
```

**Why this helps:**
- Automatically loads the skill at conversation start
- Reads the latest SKILL.md (including any updates)
- Ensures Professor Synapse has full context from your customizations

### How the Skill Works

1. **You ask for help** → Professor Synapse greets you and gathers context
2. **Assesses complexity** → Determines if this needs one agent or multiple perspectives
3. **Path A: Single Agent** (most cases)
   - Checks `agents/INDEX.md` for a matching specialist
   - If match found → Loads and summons that agent
   - If no match → Summons 🔎 Domain Researcher to research the domain, then drafts a new expert agent for review
4. **Path B: Convener Mode** (complex decisions)
   - Identifies multiple relevant perspectives
   - Hosts a structured debate among specialist agents
   - Synthesizes insights and presents options with trade-offs
5. **Persistence is explicit** → New agents or pattern updates are saved only when the user asks
6. **Packaging is optional** → Rebuild/package only when the user explicitly requests it

---

## Features

### Core Capabilities

+ **Expert Agent Summoning:** Loads existing experts or drafts new specialists tailored to your task and domain using a structured template.
+ **Contextual Understanding:** Gathers detailed information about user goals and preferences through targeted questions.
+ **Orchestrated Conversations:** Maintains clear communication between Professor Synapse and summoned agents using a defined conversation pattern.
+ **Wise Guidance:** Provides critical yet respectful challenges to help users think deeply about their goals.
+ **Intellectual Humility:** Admits uncertainty and asks clarifying questions rather than assuming.

### Advanced Features

+ **Multi-Agent Debates (Convener Protocol):** When facing complex decisions with trade-offs, Professor Synapse can convene multiple expert agents to debate from different perspectives, then synthesize their insights into actionable recommendations.

+ **Smart GitHub Updates:** Fetch updates from the canonical repository while preserving your custom agents and learned patterns. The update protocol is designed to avoid blind overwrites.
+
+ **Skill Rebuilding:** Rebuilding and packaging are explicit maintenance tasks performed only when requested.
+
+ **Pattern Learning:** Agents may propose reusable patterns and anti-patterns, but persistence requires explicit approval.
+
+ **GitHub Fetching Scripts:** Helper scripts fetch files from GitHub without auto-installing dependencies into the host environment.
+
+ **Safety Defaults:** Web content is treated as untrusted input, new agents are drafted before saving, and core skill files are not modified automatically.

---

## ChatGPT GPT

You can use the official Professor Synapse GPT by clicking [HERE](https://chatgpt.com/g/g-ucpsGCQHZ-professor-synapse)

If you'd like to edit and use Professor Synapse as your own GPT, follow these steps:

1. **Open ChatGPT**: Ensure you have access to OpenAI's ChatGPT.
2. **Create a GPT**: Go to the [GPT Editor](https://chatgpt.com/gpts/editor) and paste the prompt into your instructions.
3. **Edit**: Feel free to edit the prompt, but focus on the personality, name, persona if you're new to prompting.
4. **Start Interacting**: Begin a new chat and tell Professor Synapse what you want to accomplish.

---

## Interaction Flow

Professor Synapse uses a structured approach to help you achieve your goals:

1. **Introduction**: Greets you warmly and asks what you want to accomplish
2. **Context Gathering**: Asks targeted questions to understand your goals and preferences
3. **Agent Summoning**: Loads an expert agent or drafts one suited to your task
4. **Orchestrated Conversation**: Delegates to the expert while providing guidance
5. **Learning**: Proposes patterns and insights for future persistence

---

## Contributions and Support

Feel free to explore, customize, and innovate with Professor Synapse! Please leave a ⭐ if you found this helpful.

**Support the project:** [💖 Donate](https://donate.stripe.com/bIY4gsgDo2mJ5kkfZ6)

**For more goodies:**
- 🕸 [Website](https://www.synapticlabs.ai/)
- 📺 [Youtube](https://www.youtube.com/@synapticlabs)
- 📖 [Substack](https://professorsynapse.substack.com)
