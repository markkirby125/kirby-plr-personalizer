# Modular Dataset Architecture: Plug-and-Play Personalization

The suite uses **exactly three** canonical files. Do not invent suffixes or alternate field names. Producers: `kirby-audience-intel-profiler`, `kirby-voice-dna-extractor`, `kirby-storyline-bank`.

---

## 1. Audience Intel — `audience_profile.yaml`

Schema owned by `kirby-audience-intel-profiler`.

```yaml
---
audience_profile:
  avatar_name: "B2B Fractional CMO"
  target_market: "Solo consultants advising $2M-$10M ARR companies"
  experience_level: "Senior (Ex-VP of Marketing / Senior Agency Director)"
  lexicon_whitelist:
    - "pipeline velocity"
    - "attribution model"
  taboo_generic_terms:
    - "make sales"
    - "get clients"
  daily_friction_points:
    - "Founders micromanaging channel tactics instead of letting strategy run"
  core_objections_to_training:
    - "Generic marketing courses are insulting."
  aspirational_victory: "Four high-retainer accounts, quarterly advisory calls only."
---
```

---

## 2. Voice DNA — `voice_dna.yaml`

Schema owned by `kirby-voice-dna-extractor`.

```yaml
---
voice_dna:
  author_id: "operator_01"
  posture: "Pragmatic Practitioner (direct, zero-fluff, tough love)"
  reading_level: "Grade 7-8 (accessible, punchy, clear)"
  cadence:
    primary_sentence_length: "8-14 words"
    fragment_frequency: "High (approx 2-3 per 250 words)"
    pacing: "Fast, punchy, conversational transitions"
  lexicon:
    signature_terms: ["slog", "feast-or-famine", "operational drag"]
    taboo_banned_words: ["delve", "tapestry", "game-changer"]
    preferred_transitions: ["Look,", "Here is the truth:"]
  formatting_quirks:
    use_em_dashes: true
    use_parenthetical_asides: true
    max_paragraph_lines: 3
  vulnerability_stance: "Openly cites specific dollar losses and wasted time"
---
```

---

## 3. Storyline Bank — `storyline_bank.json`

Schema owned by `kirby-storyline-bank`. Top-level value is an **array**.

```json
[
  {
    "id": "STORY-042",
    "title": "The $8k Funnel Collapse",
    "archetype": "Expensive Mistake",
    "topics": ["funnels", "automation", "tech_stack", "launching"],
    "target_emotions": ["overwhelm", "shame", "frustration"],
    "one_sentence_hook": "I once watched $8,000 in ad spend evaporate in 48 hours because a single webhook was disconnected.",
    "narrative_beats": {
      "context": "Running a high-volume flash sale for a client in 2021.",
      "conflict": "Traffic was surging, but Stripe dashboard was dead silent.",
      "discovery": "Found a broken Zapier connection routing leads to a 404 page.",
      "resolution": "Rebuilt the pipeline with zero complex automations and salvaged the launch."
    },
    "core_lesson": "Complex automations are failure magnets; simple static pipelines protect your margins.",
    "usable_snippets": [
      "Simplicity isn't just aesthetic; it's operational insurance."
    ]
  }
]
```

---

## 4. Mix-and-match

Swap `audience_profile.yaml` or `storyline_bank.json` between runs. Do not rename the files.
