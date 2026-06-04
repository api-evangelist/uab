# Autonomous University of Barcelona (uab)

The Autonomous University of Barcelona (Universitat Autònoma de Barcelona, UAB) is a public research university in Bellaterra, near Barcelona, Spain, founded in 1968 and ranked #175 in the QS World University Rankings 2025. This repository catalogs UAB's public, machine-accessible footprint as an [APIs.json](https://apisjson.org) provider profile. UAB does not operate a formal developer portal; its strongest public, programmatic surface is the open scholarly infrastructure of its institutional repository.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/uab/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=uab-api-evangelist&utm_content=repo

## Type

- Index / Consumer / 3rd-Party

## Tags

Education, Higher Education, University, Spain, Catalonia, Open Access, Institutional Repository, OAI-PMH, Research Data

## APIs

- **DDD Digital Document Repository OAI-PMH** — OAI-PMH 2.0 metadata harvesting endpoint for the Dipòsit Digital de Documents de la UAB (Invenio platform, OpenAIRE-compliant). Base URL `https://ddd.uab.cat/oai2d`. Docs: https://www.uab.cat/en/libraries/digital-document-repository
- **CSUC Research Data Repository (CORA RDR)** — UAB research data published via the federated Catalan CSUC/CORA research data repository (FAIR, EOSC-aligned consortium platform; not a UAB-only API). Docs: https://www.uab.cat/web/research/open-access-uab/open-access-data-1345704463199.html

## Plans

- [plans/uab-plans-pricing.yml](plans/uab-plans-pricing.yml)

## Rate Limits

- [rate-limits/uab-rate-limits.yml](rate-limits/uab-rate-limits.yml)

## FinOps

- [finops/uab-finops.yml](finops/uab-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-06-03

## Common Properties

- Website: https://www.uab.cat/
- LinkedIn: https://www.linkedin.com/school/uabbarcelona/
- Plans: plans/uab-plans-pricing.yml
- Rate Limits: rate-limits/uab-rate-limits.yml
- FinOps: finops/uab-finops.yml
- Review: review.yml

## Notes

- No formal, publicly documented UAB developer portal or API program was found, and no official institutional GitHub organization for the Catalan UAB (uab.cat) was confirmed. Unrelated "uab.edu"/uabrc GitHub orgs belong to the University of Alabama at Birmingham and were deliberately excluded.
- The DDD OAI-PMH endpoint was verified live (valid Identify response, Invenio-based, OpenAIRE-compliant). Direct curl probes from the cataloging network returned 000 for some HTTPS hosts due to apparent TLS/bot filtering; those surfaces were verified via independent fetch.
- Student academic services (SIA, sia.uab.es) are gated login portals without public API documentation.
- No endpoints, keys, or specifications were fabricated; only confirmed public surfaces are cataloged.

## Maintainers

- Kin Lane — kin@apievangelist.com
