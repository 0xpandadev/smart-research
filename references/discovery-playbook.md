# Discovery Playbook

Use discovery to build the source universe. Do not treat any single discovery channel as complete.

## Channels

- Search provider results: broad web, news, images, videos, discussions.
- Direct primary navigation: official company, IR, filings, government, regulator, standards, docs, GitHub.
- Document search: PDF, annual report, investor presentation, whitepaper, deck, benchmark, survey.
- Specialist search: trade media, journals, analyst/consulting reports, professional associations.
- Weak-signal search: Reddit, X, HN, forums, reviews, comments, Discord/Slack archives only when public and accessible.
- Contradiction search: negative evidence, customer complaints, incidents, lawsuits, regulatory action, failed adoption.

## Query Design

Generate query families:

- Entity plus source type: `<company> annual report`, `<market> regulator`, `<technology> benchmark pdf`.
- Problem language: `<customer pain> complaint`, `<workflow> reddit`, `<product> alternative`.
- Evidence language: `market size`, `pricing`, `adoption`, `case study`, `churn`, `outage`, `security`, `regulation`.
- Primary source targeting: `site:sec.gov`, `site:edinet-fsa.go.jp`, `site:ir.<company>`, `site:gov`, `site:edu`, `filetype:pdf`.
- Counterevidence: `criticism`, `lawsuit`, `failed`, `risks`, `limitations`, `why not`, `problems`.

## Brave-Or-Similar Use

Use Brave or other search APIs as discovery channels only. Do not let the result ranking define the evidence universe. Verify important claims through primary or independent sources.

Use freshness/news/image/video/discussion search when the user needs current information, specialist coverage, visual material, video context, or community signals.
