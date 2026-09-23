# Autonomous University of Barcelona (uab)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

The Universitat Autònoma de Barcelona (UAB) is a public research university in Bellaterra, Catalonia, Spain, founded in 1968. This repository catalogs UAB's public, machine-accessible footprint as an [APIs.json](https://apisjson.org) provider profile, re-profiled on 2026-09-01 under the API Evangelist university pipeline, which settles **who operates** each surface before recording it.

UAB is one of the few institutions in this cohort whose programmable footprint is genuinely its own. It runs four OAI-PMH 2.0 endpoints and a SAML 2.0 identity provider on its own RIPE allocation. It publishes no specification for any of them, and it operates no developer programme.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/uab/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=uab-api-evangelist&utm_content=repo

## Type

- university / Public Research University / Index / Consumer / 3rd-Party

## Tags

Education, Higher Education, University, Spain, Catalonia, Research, Open Access, Institutional Repository, Research Repository, Research Data, OAI-PMH, Identity Federation, Scholarly Publishing

## Surfaces, by operator

Every entry carries an `x-operator`. `institution` means UAB runs the thing the entry describes; `tenant`, `federation` and `registry` mean the relationship is real and UAB's while the contract belongs to someone else.

### institution — UAB's own (7)

- **DDD — Dipòsit Digital de Documents (OAI-PMH 2.0)** — `https://ddd.uab.cat/oai2d`. 221,931 records, 18 sets, four metadata prefixes (`oai_dc`, `marcxml`, `edm`, `oai_openaire`). Identify, ListSets, ListMetadataFormats, ListIdentifiers and GetRecord all verified 200.
- **DDD Invenio search and export** — `https://ddd.uab.cat/search`. MARC21 XML, Dublin Core and BibTeX export, anonymous, no key.
- **Traces — Catalan language and literature database (OAI-PMH 2.0)** — `https://traces.uab.cat/oai2d`.
- **IFMuC — Inventari dels Fons Musicals de Catalunya (OAI-PMH 2.0)** — `https://ifmuc.uab.cat/oai2d`.
- **Revistes UAB — self-hosted Open Journal Systems** — per-journal OAI-PMH endpoints, e.g. `https://revistes.uab.cat/catJL/oai`. UAB runs the instance; PKP's generic REST contract is not saved here.
- **UAB SSO — SAML 2.0 Identity Provider** — `https://sso.uab.cat/cas/idp/metadata`. A complete, self-published EntityDescriptor from UAB's own Apereo CAS server. The one institution-published machine-readable contract in this profile.
- **UAB Central Authentication Service (CAS 3.0)** — `https://sso.uab.cat/cas/`.

### federation (1)

- **UAB in SIR / eduGAIN** — entityID `https://www.rediris.es/sir/uabidp`, scope `uab.es`, present in the RedIRIS SIR aggregate and in eduGAIN as entity 680530. UAB's identity, RedIRIS's engineering — every endpoint terminates on `sir.rediris.es`.

### tenant (1)

- **CORA Repositori de Dades de Recerca — UAB collection** — `https://dataverse.csuc.cat/dataverse/UAB`, 567 datasets, contact `ddd.bib@uab.cat`, DOIs under CSUC's prefix 10.34810. The data is UAB's; the Dataverse platform, contract and DOI registration are CSUC's, and CSUC's specification is deliberately not saved here.

### registry (2)

- **Crossref** — member 3612, DOI prefix 10.5565, 23,089 deposited DOIs.
- **ROR** — https://ror.org/052g8jq94.

## Artifacts

- [openapi/uab-ddd-openapi.yml](openapi/uab-ddd-openapi.yml) — **derived by API Evangelist**, not published by UAB. Written from live probes; pristine copy in [openapi/_original/](openapi/_original/).
- [conformance/uab-conformance.yml](conformance/uab-conformance.yml) — `education` regime standards. Evidenced: `oai-pmh`, `saml`, `shibboleth`, `crossref` (institution); `datacite` (tenant).
- [identity-federation/uab-identity-federation.yml](identity-federation/uab-identity-federation.yml) — both identity entities, with archived metadata.
- [authentication/uab-authentication.yml](authentication/uab-authentication.yml)
- [examples/uab-examples.yml](examples/uab-examples.yml) — eight verbatim captured responses.
- [json-ld/uab-context.jsonld](json-ld/uab-context.jsonld)
- [plans/uab-plans-pricing.yml](plans/uab-plans-pricing.yml) · [rate-limits/uab-rate-limits.yml](rate-limits/uab-rate-limits.yml) · [finops/uab-finops.yml](finops/uab-finops.yml) · [security/uab-domain-security.yml](security/uab-domain-security.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-09-01

## Common Properties

- Website: https://www.uab.cat/
- Documentation: https://www.uab.cat/en/libraries/digital-document-repository
- Research repository: https://ddd.uab.cat/
- Open science / research data: https://www.uab.cat/ca/ciencia-oberta/dades-de-recerca-obert
- AI policy: https://www.uab.cat/ca/etica-recerca/artificial
- Legal notice: https://www.uab.cat/web/about-the-uab/itineraries/legal-notice-1345668684716.html
- Privacy: https://www.uab.cat/web/la-uab/itineraris/proteccio-de-dades-1345668257177.html
- LinkedIn: https://www.linkedin.com/school/uabbarcelona/
- Review: review.yml

## Notes

- **No specification is published by UAB for anything.** The OpenAPI in this repository is derived by API Evangelist from live probes and is marked `method: derived` throughout. It must not be read as a UAB contract.
- **No developer programme.** No API keys, no OAuth authorization server (CAS's OIDC module returns 404 on both discovery paths and on `/cas/oidc/jwks`), no registration, no `llms.txt`. `api.uab.cat`, `data.uab.cat`, `opendata.uab.cat`, `dades.uab.cat`, `idp.uab.cat` and `cataleg.uab.cat` do not resolve.
- **Operator was settled by IP ownership, not hostname.** `ddd`, `traces`, `ifmuc`, `revistes`, `sso` and `www` all resolve inside 158.109.0.0/16 — RIPE netname `XIUAB`, "Xarxa Informatica de la Universitat Autonoma de Barcelona". `dataverse.csuc.cat` resolves into `CESCANET` / "CSUC Services", and `sir.rediris.es` into `REDIRIS`.
- **A dead pointer was removed.** The previous profile's only research-data pointer returned HTTP 200 with a body byte-identical to UAB's 404 page — a soft-404 reading as a live claim.
- **Searching in Catalan was load-bearing.** The AI policy exists only on the Catalan surface; Traces and IFMuC were found through DDD's own OAI-PMH `friends` declaration; and UAB's eduGAIN entity is findable only by its RedIRIS-namespaced entityID, since every `uab` host in eduGAIN belongs to the University of Alabama at Birmingham or Universidade Aberta.
- No official institutional GitHub organisation for the Catalan UAB (`uab.cat`) was found. `github.com/UAb` is Universidade Aberta; `uab.edu` / `uabrc` orgs belong to Alabama-Birmingham. All deliberately excluded.
- No endpoints, keys, or specifications were fabricated; only confirmed public surfaces are cataloged.

## Maintainers

- Kin Lane — kin@apievangelist.com
