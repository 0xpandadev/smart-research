# Research Modes

Select a mode automatically unless the user specifies one.

## quick

Use for orientation, definitions, current status, or a short source-backed answer. Return the initial source map, 3-5 strongest sources, and uncertainty.

## standard

Use for most research. Create a focused research map, search across multiple source types, triangulate key claims, preserve useful original wording, and produce a concise evidence-backed research brief.

## deep

Use when PDFs, filings, decks, tables, figures, documentation, or long reports matter. Extract content deeply, preserve source metadata and original excerpts, compare across documents, and identify what each document proves or fails to prove.

## wild

Use when the task asks for non-obvious signals, market reality, user sentiment, emerging behavior, or messy public evidence. Include Reddit, X, HN, forums, GitHub issues, comments, video captions, niche blogs, and specialist communities when available. Treat all outputs as weak signals until verified.

## ultra

Use for high-stakes, complex, or long-horizon research. Combine `deep` and `wild`, maintain a research ledger, search for disconfirming evidence, and produce a transparent evidence pack. Add recommendations only when requested.

## Auto-Escalation Defaults

Default to `deep` or `ultra` when the topic involves:

- Investment, finance, company diligence, market analysis, or valuation
- AI, technology strategy, infrastructure, developer adoption, or technical due diligence
- Competitor analysis, market structure, business strategy, or product strategy
- Regulation, geopolitics, safety, security, or public claims
- Any answer that may affect spending, risk, reputation, or strategic decisions

Use the user's requested output shape if provided. The mode controls research depth, not whether the final answer must be a table, memo, bullets, or report.

## Escalation

Escalate mode when:

- Primary sources disagree
- The user asks for investment, strategy, diligence, regulation, safety, or financial implications
- Important sources are PDFs/decks/images rather than HTML
- Weak signals contradict official narratives
- The answer would materially affect spend, risk, strategy, safety, or public claims
