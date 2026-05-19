# Ingestion Playbook

Use ingestion to read sources deeply after discovery.

## Web Pages

Extract:

- Main text, author, publisher, date, title, links, tables, figures, captions, and quoted claims
- Source type and likely bias
- Claims supported by data versus claims that are commentary

## PDFs And Documents

For reports, decks, filings, whitepapers, and manuals:

- Extract text in reading order.
- Preserve tables as tables when possible.
- Identify charts, matrices, architecture diagrams, stacks, market maps, and page numbers.
- Capture document metadata: title, organization, date, version, geography, methodology.
- If text extraction is weak, use OCR or image-level reading when available.
- For important tables, check units, denominators, time periods, and footnotes.

## Firecrawl-Or-Similar Use

When available, use page scraping for single pages, parse for PDFs/documents, map for site structure, and limited crawl for bounded domains. Escalate to browser/interact only with explicit approval.

Safe order:

1. Search/discover
2. Scrape selected pages
3. Parse documents/PDFs
4. Map site structure
5. Limited crawl with domain and page limits
6. Browser/interact only after approval

## Evidence Capture

For every important source, record:

- URL or source identifier
- Date published or accessed
- Source tier
- Key facts
- Key estimates
- Useful quotes or table values
- Contradictions or caveats
- Confidence
