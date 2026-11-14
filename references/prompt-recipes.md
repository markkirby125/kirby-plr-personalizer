# Master Prompt Recipes for Two-Way PLR Personalization

These standardized prompt recipes are calibrated for precision execution across multiple AI models (Claude, GPT-4o, Gemini, Cursor, etc.).

---

## Recipe 1: Master Framework Fusion Prompt

```markdown
You are a senior direct-response content strategist and master ghostwriter. 
Transform the raw Private Label Rights (PLR) text below into a high-authority, authentic article tuned specifically for {{TARGET_AUDIENCE}}.

### CONTEXT & INPUTS:
1. RAW PLR CONTENT:
"""
{{INSERT_RAW_PLR_TEXT}}
"""

2. TARGET AUDIENCE INTEL:
- Subniche: {{TARGET_SUBNICHE}}
- Day-to-day operational realities: {{DAILY_REALITIES}}
- Insider Lexicon / Jargon to include: {{LEXICON_LIST}}
- Taboo generic phrases to ban: {{BANNED_PHRASES}}

3. AUTHOR VOICE & STORYLINE:
- Tone: {{VOICE_STYLE}} (e.g., direct, candid, punchy, mentor-style)
- Micro-Story / Experience anchor:
"""
{{INSERT_AUTHOR_STORY_OR_ANECDOTE}}
"""

### RULES OF EXECUTION:
1. Strip all generic throat-clearing openings. Hook the reader immediately with an audience-specific problem or tension.
2. Weave the Author's micro-story into the text as organic proof. Do not isolate it into a detached "Let me tell you a story" sidebar.
3. Translate all educational principles from the raw PLR into the concrete tools, metrics, and daily friction experienced by {{TARGET_SUBNICHE}}.
4. Use varied sentence rhythm: mix short, punchy statements with rhythmic explanatory sentences.
5. Reorder/restructure boilerplate PLR section skeletons and replace stock-photo placeholders instead of swapping nouns in original headings.
6. Zero-Invention Guardrail: Never fabricate dates, metrics, or scars missing from the Author Storyline input; emit `[VERIFY: insert real metric/story]` where proof is absent.
7. For web-published guides: frame `H2`/`H3`s as exact buyer-question/fan-out queries with verbatim tool/competitor names, include an explicit trade-off or competitor concession where warranted, and optionally add a contextualized 4-Slot Brand Proof Passage (`[BRAND NAME] + [SPECIFIC PROOF] + [THE SERVICE] + [WHY IT MATTERS TO THE READER]`, 2–3 sentences with real dated numbers).
8. End with a clear, pragmatic directive for the reader.
```

---

## Recipe 2: The Socratic Memory-Extraction Prompt

```markdown
I want to personalize this PLR piece on {{TOPIC}} with my own voice and personal stories, but I haven't written out my notes yet.
Read this raw text:
"""
{{INSERT_RAW_PLR_TEXT}}
"""

Ask me 3 sharp, specific questions about my real-world experience, mistakes, and contrarian opinions related to the central advice in this text. 
Format each question so I can answer in just 1-2 bullet points.
Once I answer, you will use those answers to execute Framework Fusion.
```

---

## Recipe 3: Batch De-Genericizer & Subniche Translator

```markdown
Take the following raw educational outline/subheadings:
"""
{{INSERT_SUBHEADINGS_OR_OUTLINE}}
"""

1. Reorder and restructure the boilerplate PLR section skeleton so the flow reflects {{TARGET_SUBNICHE}}'s actual decision path (do not merely swap nouns inside the original outline order).
2. Rewrite subheadings as exact buyer-question / fan-out H2/H3s where applicable, naming verbatim tools, platforms, or competitors.
3. Replace every broad term ("business", "success", "results", "growth") with precise industry equivalents (e.g. for agency owners: "retainers", "churn rate", "scope creep", "outbound volume").
4. Strip any stock-photo placeholders and specify domain-authentic visual callouts (e.g., workflow diagrams, annotated tool screens, checklists).
5. Ensure each bullet establishes high topical authority without inventing unverified metrics.
```
