---
name: kirby-plr-personalizer
description: "Use when rewriting raw PLR with audience intel plus Voice DNA and storylines."
category: writing
triggers: [personalize-plr, rewrite-plr, de-genericize, plr-makeover, framework-fusion, plr-slop]
---

# SOP: Master Two-Way PLR Personalization & Framework Fusion

> Standard Operating Procedure for rescuing generic, neutral Private Label Rights (PLR) content from the "PLR Pile-Up" and transforming it into high-converting, authoritative, and distinctive intellectual property using the Two-Way Personalization Engine.

---

## 1. The Two Vectors of Personalization

Personalization fails when operators attempt to "just rewrite" text without structured constraints. True transformation requires two distinct inputs:

### Vector 1: Audience-Driven Intel (Subniche Filtering)
Tuning broad concepts to the precise reality of a targeted micro-audience:
* **Broad PLR Concept:** *"Setting priorities is an important step in getting more done."*
* **Audience Tuning (e.g., Solo eCommerce Store Owners):** *"When peak holiday shipping hits and you have 47 unfulfilled orders on Shopify, prioritizing supplier check-ins over tweaking your banner image is what keeps you from drowning."*
* **Mechanics:** Injects native industry lexicon, addresses actual operational friction, replaces hypothetical generalizations with domain-specific stakes.

### Vector 2: Voice & Storyline Infusion (Human Handprint)
Injecting the author's lived experiences, failures, tone quirks, and perspective:
* **Broad PLR Concept:** *"Starting an email list requires consistency."*
* **Voice/Story Tuning:** *"Back in 2019, I let my newsletter sit silent for four months because I thought I needed a 10-part masterclass ready. When I finally hit send on a raw 3-paragraph update, I made $1,200 in 24 hours. The lesson? Perfection is a coward's excuse."*
* **Mechanics:** Drops in micro-stories, business scars, conversational cadence, signature phrases, and personal stance.

---

## 2. The 4-Step Personalization Lifecycle

```
[Phase 1: Input Ingestion]
  ├── Ingest Raw PLR Asset
  └── Tag Core Concept & Subtopics
          │
          ▼
[Phase 2: Dataset Assembly]
  ├── Select/Generate Audience Intel Dataset (Vector 1)
  └── Select/Generate Voice DNA & Storyline Bank (Vector 2)
          │
          ▼
[Phase 3: Framework Fusion Execution]
  ├── Run Single-Pass Fusion Prompt
  └── Preserve Educational Meat / Strip Generic Slop
          │
          ▼
[Phase 4: Conformance & Diagnostic Audit]
  ├── Audit against 15-point diagnostic checklist
  └── Ensure zero lingering PLR fingerprints
```

### Phase 1: Input Ingestion
1. Read the source PLR text.
2. Identify the **Core Educational Value**: Strip fluff introductions ("In today's fast-paced world..."). Isolate the underlying steps, frameworks, or advice.

### Phase 2: Dataset Assembly
Before executing the rewrite, load these three canonical files (same names everywhere in the suite):
* `audience_profile.yaml` — avatar, `lexicon_whitelist`, `taboo_generic_terms`, `daily_friction_points`. Producer: `kirby-audience-intel-profiler`.
* `voice_dna.yaml` — posture, cadence, signature terms, taboo list. Producer: `kirby-voice-dna-extractor`.
* `storyline_bank.json` — array of archetype entries with `topics`, `target_emotions`, `narrative_beats`. Producer: `kirby-storyline-bank`.
* If a file is missing, invoke the producer skill and write that filename. Do not invent a fourth filename.

### Phase 3: Framework Fusion Execution
Execute the single-pass fusion using the following directives:

**Inputs Required:**
1. **RAW PLR:** {{INSERT_RAW_PLR_TEXT}}
2. **AUDIENCE INTEL:** Target Audience ({{TARGET_SUBNICHE}}) and Insider Lexicon / Real-world stakes ({{LEXICON_AND_PAIN_POINTS}})
3. **AUTHOR VOICE & STORYLINE:** Voice Tone / Cadence ({{VOICE_DNA_SUMMARY}}) and Personal Story / Micro-Anecdote ({{ANECDOTE_OR_LESSON}})

**Execution Directives:**
1. Retain the core actionable advice or instructional framework from the raw PLR.
2. Eliminate all generic, corporate, or filler introductory phrases.
3. Anchor all explanations directly into the Target Audience's daily operational reality using their vocabulary.
4. Seamlessly weave the Author's micro-story or lesson into the narrative as proof/context, ensuring it feels organic rather than bolted-on.
5. Match the requested voice cadence (sentence length variety, conversational tone, direct perspective).

### Phase 4: Conformance & Diagnostic Audit
Verify the output meets the anti-slop threshold:
- [ ] Are any broad placeholders ("entrepreneurs", "success", "businesses") remaining?
- [ ] Does the story flow logically into the instructional takeaway without clashing?
- [ ] Is the reading level and terminology authentic to the subniche?
- [ ] If any diagnostic defect is flagged, route to `kirby-plr-diagnostic-debugger`.

---

## 3. Operational Modes: 2-Minute Makeover vs. Batch Pipeline

### The 2-Minute Makeover (Rapid Ad-Hoc Execution)
When a single piece needs immediate publishing:
1. Copy raw PLR paragraph/article.
2. Feed into the **On-The-Fly Storyline Infusion Prompt** (see [references/prompt-recipes.md](references/prompt-recipes.md)).
3. Request 2 candidate variations (conversational vs. authoritative).
4. Review, select, publish.

### The Batch Scaling System (10 Pieces Per Day)
To eliminate the PLR backlog:
1. **Modular Dataset Pre-loading:** Maintain persistent `audience_profile.yaml`, `voice_dna.yaml`, and `storyline_bank.json`.
2. **Chunking:** Break large PLR ebooks/reports into modular chapters or 500-word standalone topics.
3. **Pipelined Execution:** Run batch transforms through Framework Fusion, outputting formatted drafts ready for distribution.

---

## 4. Modular Skill Ecosystem & Dispatcher Routing

This skill acts as the master conductor. Route sub-tasks to specialized companion skills:

| Task / Domain | Target Companion Skill |
|---|---|
| Deep Avatar Profiling & Lexicon Extraction | `kirby-audience-intel-profiler` |
| Author Style, Cadence & Tone Codification | `kirby-voice-dna-extractor` |
| Curating & Querying Personal Experience Banks | `kirby-storyline-bank` |
| Converting PLR into 10 Email Sequence Types | `kirby-plr-email-sequences` |
| Turning Informational PLR into Direct-Response Sales Pages | `kirby-plr-sales-converter` |
| Cascading 1 Asset into 12 Platform-Native Posts | `kirby-plr-omnichannel-repurposer` |
| Repairing Tone Drift, Forced Stories, or Residual PLR Slop | `kirby-plr-diagnostic-debugger` |

---

## 5. Reference Documentation Index

For deep operational templates and prompt libraries, consult:
* [references/framework-fusion-guide.md](references/framework-fusion-guide.md) — Comprehensive comparative analysis and fusion examples.
* [references/modular-datasets.md](references/modular-datasets.md) — Schemas for Audience Datasets and Storyline Banks.
* [references/two-minute-makeover.md](references/two-minute-makeover.md) — High-velocity workflows for rapid deployment.
* [references/prompt-recipes.md](references/prompt-recipes.md) — Exact master prompt templates.
