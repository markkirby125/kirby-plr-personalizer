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
5. End with a clear, pragmatic directive for the reader.
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

Rewrite each subheading and summary bullet to speak directly to {{TARGET_SUBNICHE}}.
Replace every broad term ("business", "success", "results", "growth") with precise industry equivalents (e.g. for agency owners: "retainers", "churn rate", "scope creep", "outbound volume").
Ensure each bullet establishes high topical authority.
```
