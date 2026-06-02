# Exhaustive Learning Map Extractor — Claude Skill

A Claude Skill for converting transcripts, lectures, notes, research dumps, meeting transcripts, and other long unstructured text into **exhaustive, zero-detail-loss learning maps**.

This skill is designed for users who do not want a normal summary. Instead, it restructures source material into a detailed, navigable learning map while preserving definitions, examples, caveats, numbers, relationships, contradictions, edge cases, and source anchors.

---

## What This Skill Does

The **Exhaustive Learning Map Extractor** helps Claude transform messy or lengthy material into structured learning assets such as:

- Markdown learning maps
- JSON ontologies
- Mermaid mindmaps
- Knowledge graph-style edge lists
- Structured study outlines

Its core purpose is **faithful transformation, not compression**.

A summary asks:

> What matters most?

This skill asks:

> What is present in the source, and how does it all connect?

---

## Key Features

- Preserves major topics, subtopics, definitions, named entities, dates, numbers, examples, caveats, warnings, limitations, and edge cases.
- Tracks relationships such as cause and effect, prerequisites, dependencies, contrasts, contradictions, workflows, and hierarchies.
- Avoids adding outside knowledge unless explicitly requested.
- Supports multiple output formats including Markdown, JSON, Mermaid, and knowledge graph tables.
- Handles long inputs by processing material section by section instead of pretending the extraction is complete.
- Includes verification checks for omitted numbers, examples, caveats, definitions, and relationships.

---

## Files

```text
exhaustive-learning-map-extractor/
├── SKILL.md
├── README.md
└── references/
    └── RESEARCH_NOTES.md
