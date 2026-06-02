# Research Notes: Exhaustive Learning Map Extraction Skill

These notes are the research foundation supplied by the user. The operational Claude Skill is in `../SKILL.md`.

## Core Design Thesis

A learning map extraction system must reject summarization and instead perform zero-detail-loss transformation from unstructured transcripts into structured maps, JSON ontologies, Mermaid diagrams, Markdown outlines, or knowledge graphs.

## Main Architecture Ideas Preserved

- Treat ordinary LLM extraction as a kind of semantic downsampling.
- Counteract detail loss through multiple extraction passes.
- Use strict task directives and output schemas.
- Use transcript boundaries and structured sections.
- Preserve factual fidelity through source references.
- Use macro, entity, relationship, and micro-detail sweeps.
- Merge duplicates without deleting nuance.
- Verify against omissions and hallucinations.
- Prefer Markdown for very long exhaustive maps.
- Use JSON for programmatic ontology output.
- Use Mermaid for visual topological rendering when size allows.

## Key Failure Modes Addressed

- Lost-in-the-middle attention degradation.
- Over-summarization.
- Vague instructions such as “be detailed.”
- Hidden multi-step dependencies.
- No explicit output scope.
- Mermaid formatting drift.
- JSON invalidity.
- Confabulation.
- Shallow verification loops.
- Deduplication that deletes useful nuance.

## Important Implementation Choices

The final `SKILL.md` avoids unsupported claims about hidden chain-of-thought access or API-only settings. Instead, it turns the research into practical behavioral instructions that work as a Claude Skill:

- extract in phases;
- cite source anchors;
- make omissions visible;
- use deterministic schemas;
- verify before final output;
- fall back gracefully when outputs are too large.
