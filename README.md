# Opus

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

OpusClip (Opus) is an AI video platform that turns long-form videos into short-form, viral clips and publishes them to social platforms. The OpusClip API lets developers submit a source video by URL or upload, create a clipping project, tune curation/import/render preferences, apply brand templates, retrieve exportable clips and transcripts, organize clips into collections, run censor and generative thumbnail jobs, and generate, publish, or schedule social posts to connected accounts. The API is REST over JSON at https://api.opus.pro, authenticated with a bearer API key, with HMAC-signed webhooks, page-based pagination, and a hosted MCP server plus an Agent Skill for agent-native access. API access is available on the Pro (Beta), Max, and Business plans.

**Areas:** Company · Frontier Tech · Video · Artificial Intelligence · Video Editing · Short-Form Video · Content Creation · Social Media · Media · Agents

## Opus on APIs.io

Everything profiled for Opus is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/opus/](https://apis.io/providers/opus/)** — or go straight to one of the APIs or properties below.

### APIs (9)

- [Opus Brand Templates API](https://apis.io/apis/opus/opus-brand-templates-api/) — The brand-templates API from Opus — 1 operation(s) for brand-templates.
- [Opus Censor Jobs API](https://apis.io/apis/opus/opus-censor-jobs-api/) — The censor-jobs API from Opus — 2 operation(s) for censor-jobs.
- [Opus Clip Project API](https://apis.io/apis/opus/opus-clip-project-api/) — The clip-project API from Opus — 3 operation(s) for clip-project.
- [Opus Collection API](https://apis.io/apis/opus/opus-collection-api/) — The collection API from Opus — 3 operation(s) for collection.
- [Opus Collection Content API](https://apis.io/apis/opus/opus-collection-content-api/) — The collection-content API from Opus — 2 operation(s) for collection-content.
- [Opus ExportableClip API](https://apis.io/apis/opus/opus-exportableclip-api/) — The ExportableClip API from Opus — 1 operation(s) for exportableclip.
- [Opus Generative Jobs API](https://apis.io/apis/opus/opus-generative-jobs-api/) — The generative-jobs API from Opus — 2 operation(s) for generative-jobs.
- [Opus Social Posting API](https://apis.io/apis/opus/opus-social-posting-api/) — The social-posting API from Opus — 6 operation(s) for social-posting.
- [Opus Transcripts API](https://apis.io/apis/opus/opus-transcripts-api/) — The transcripts API from Opus — 1 operation(s) for transcripts.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Arazzo workflows (2)

Multi-step workflows that chain operations into a business task.

- [OpusClip — clip a video and export clips](https://apis.io/arazzos/opus/opus-clip-and-export/)
- [OpusClip — clip a video and publish to social](https://apis.io/arazzos/opus/opus-clip-and-publish/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [opusclip](https://apis.io/servers/opus/opusclip/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Opus Agentic Access](https://apis.io/agentic-access/opus/opus-agentic-access/)

#### Collections (11)

Postman and Open Collection request collections.

- [Clip brand-templates API](https://apis.io/collections/opus/open-opus-brand-templates-api/)
- [Clip brand-templates censor-jobs API](https://apis.io/collections/opus/open-opus-censor-jobs-api/)
- [Clip brand-templates clip-project API](https://apis.io/collections/opus/open-opus-clip-project-api/)
- [Clip brand-templates collection API](https://apis.io/collections/opus/open-opus-collection-api/)
- [Clip brand-templates collection-content API](https://apis.io/collections/opus/open-opus-collection-content-api/)
- [Clip brand-templates enterprise API](https://apis.io/collections/opus/open-opus-enterprise-api/)
- [Clip brand-templates exportable-clips API](https://apis.io/collections/opus/open-opus-exportable-clips-api/)
- [Clip brand-templates ExportableClip API](https://apis.io/collections/opus/open-opus-exportableclip-api/)
- [Clip brand-templates generative-jobs API](https://apis.io/collections/opus/open-opus-generative-jobs-api/)
- [Clip brand-templates social-posting API](https://apis.io/collections/opus/open-opus-social-posting-api/)
- [Clip brand-templates transcripts API](https://apis.io/collections/opus/open-opus-transcripts-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Opus Openapi Overlay](https://apis.io/overlays/opus/opus-openapi-overlay/)

#### Security (4)

Authentication, trust centre, and vulnerability disclosure.

- [Opus Authentication](https://apis.io/security/opus/opus-authentication/)
- [Opus Domain Security](https://apis.io/security/opus/opus-domain-security/)
- [Opus Trust Center](https://apis.io/security/opus/opus-trust-center/)
- [Opus Vulnerability Disclosure](https://apis.io/security/opus/opus-vulnerability-disclosure/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Opus Plans Pricing](https://apis.io/plans/opus/opus-plans-pricing/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.opus.pro/)
- [Documentation](https://help.opus.pro/api-reference/overview)
- [Getting started](https://help.opus.pro/api-reference/quickstart)
- [API reference](https://help.opus.pro/api-reference/overview)
- [Pricing](https://www.opus.pro/pricing)
- [Sign up](https://clip.opus.pro/dashboard)
- [Support](https://www.opus.pro/contact-support)
- [Blog](https://www.opus.pro/blog)
- [Compliance](https://trust.opus.pro/)
- [Terms of service](https://www.opus.pro/terms-of-service)
- [Privacy policy](https://www.opus.pro/privacy-policy)
- [GitHub](https://github.com/opus-pro)
- [Status](https://status.opus.pro)

## API Evangelist rating

**Kin Score 54.1** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 75.0 |
| Contract quality | 44.0 |
| Contract governance | 4.5 |
| Operational transparency | 28.9 |
| Developer ergonomics | 66.1 |
| Access clarity | 84.2 |

**Agent readiness 53.4** — agent-ready (gated down from agent-native)

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | verified |
| Auth Clarity | served (partial credit) |
| Idempotency | — |
| Error Semantics | derived (partial credit) |
| OpenAPI Examples | partial |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | unknown |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | served (partial credit) |
| Protected Resource Metadata | verified |
| Dynamic Client Registration | yes |
| Agentic Commerce | — |
| Pagination Ratio | — |
| Operation Distinctiveness | distinct |

**Regulatory alignment 28.2** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/opus/](https://apis.io/providers/opus/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Opus: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/opus/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
