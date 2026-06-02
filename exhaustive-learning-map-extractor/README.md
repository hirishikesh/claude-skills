# Exhaustive Learning Map Extractor — Claude Skill

Upload this folder or ZIP as a Claude Skill.

## What it does

This skill turns pasted transcripts, lectures, research dumps, notes, and long unstructured text into exhaustive learning maps.

It is designed to avoid the usual LLM failure mode of summarizing too aggressively. It instructs Claude to preserve details, definitions, numbers, caveats, relationships, examples, contradictions, and source anchors.

## Files

- `SKILL.md` — the actual Claude Skill file.
- `references/RESEARCH_NOTES.md` — your original research foundation, kept for future improvement.

## Suggested invocation

After uploading, ask Claude:

> Use the exhaustive-learning-map-extractor skill. Turn this transcript into a zero-detail-loss learning map. Give me Markdown first, then a Mermaid overview.

## Best use

Paste one transcript or section at a time for maximum coverage. For very long material, ask Claude to process it section-by-section and continue from the previous map.
