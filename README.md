# Wyndham Hotels & Resorts

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

Wyndham Hotels & Resorts, Inc. (NYSE: WH) is the world's largest hotel franchising company by number of properties, with over 8,300 affiliated hotels and approximately 869,000 rooms across roughly 25 brands in 95+ countries, licensed to more than 6,200 franchisees. Headquartered in Parsippany, New Jersey, its home market is the United States. Wyndham does not operate most of its hotels — it franchises brands (Days Inn, Super 8, Ramada, La Quinta, Microtel, Baymont, Howard Johnson, Travelodge, Wingate, Wyndham, Wyndham Grand, Trademark Collection, TRYP, Dolce, ECHO Suites and others) and sells the demand that flows through them. It sits in the distribution chain as a franchisor and demand aggregator rather than as a distribution platform: inventory reaches buyers through Wyndham's own brand.com sites and Wyndham Rewards, through GDS chain codes under master chain code WR, and through third-party online travel agents, with the central reservation layer supplied by Sabre Hospitality's SynXis CRS under a relationship Sabre publicly renewed in July 2024. There is no travel API: no developer portal, no API documentation, no OpenAPI, and no property, rate, availability, reservation, loyalty or folio surface is machine-readable anywhere. developer., developers., docs. and api. subdomains do not resolve; /developers, /api, /docs, /openapi.json, /swagger.json and /api-docs all return 404, and mcp.wyndhamhotels.com resolves with a valid certificate but serves an Akamai 503 on every path. The Terms of Use (effective 2026-03-12) affirmatively prohibit robots, spiders, meta-searching and automated access, and separately prohibit automated access to Wyndham's AI Search. What a second enrichment round did find on 2026-07-28 is undocumented CMS infrastructure that is nonetheless genuinely live: www.wyndhambusiness.com and development.wyndhamhotels.com both run WordPress on WP Engine and leave the WordPress REST API anonymously readable (309 and 403 registered routes, with JSON Schema available by HTTP OPTIONS), and three WordPress MCP adapter routes are registered across the two estates — one of them, on www.wyndhambusiness.com, bound to a real OAuth 2.1 authorization server with RFC 8414 and RFC 9728 discovery metadata, mandatory PKCE S256 and a single `mcp` scope, returning a standards-correct 401 bearer challenge to anonymous callers. None of it is documented, supported, or usable without a credential Wyndham issues to no third party, and none of it carries hotel data. The integration surface that matters is still reached only through a franchise agreement, a commercial distribution agreement, or Sabre.

**Areas:** Travel · United States · Hospitality · Hotels · Booking · Franchising · Distribution · Loyalty · GDS

## Wyndham Hotels & Resorts on APIs.io

Everything profiled for Wyndham Hotels & Resorts is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/wyndham-hotels/](https://apis.io/providers/wyndham-hotels/)** — or go straight to one of the APIs or properties below.

### APIs (3)

- [Wyndham Hotels & Resorts Website (WordPress REST, www.wyndhambusiness.com)](https://apis.io/apis/wyndham-hotels/wyndhambusiness-com-website-wordpress-rest/) — The public WordPress REST API (wp-json) of the Wyndham Hotels & Resorts website at www.wyndhambusiness.com: the route index of the site's content management…
- [Wyndham Hotels & Resorts Website (WordPress REST, development.wyndhamhotels.com)](https://apis.io/apis/wyndham-hotels/development-wyndhamhotels-com-website-wordpress-rest/) — The public WordPress REST API (wp-json) of the Wyndham Hotels & Resorts website at development.wyndhamhotels.com: the route index of the site's content…
- [Wyndham Business WordPress MCP Server (OAuth-gated)](https://apis.io/apis/wyndham-hotels/wyndham-business-mcp-server/) — A WordPress MCP adapter is registered on www.wyndhambusiness.com in the `mcp` namespace alongside wp-abilities/v1, and — unlike most WordPress MCP installs…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [wyndham-hotels-mcp.yml](https://apis.io/servers/wyndham-hotels/wyndham-hotels-mcp-yml/)

#### JSON Schema (11)

The data models the API reads and writes.

- [Moved to /providers/wyndham-hotels/](https://apis.io/schemas/wyndham-hotels/wyndham-hotels-wp-v2-categories/)
- [Moved to /providers/wyndham-hotels/](https://apis.io/schemas/wyndham-hotels/wyndham-hotels-wp-v2-comments/)
- [Moved to /providers/wyndham-hotels/](https://apis.io/schemas/wyndham-hotels/wyndham-hotels-wp-v2-media/)
- [Moved to /providers/wyndham-hotels/](https://apis.io/schemas/wyndham-hotels/wyndham-hotels-wp-v2-pages/)
- [Moved to /providers/wyndham-hotels/](https://apis.io/schemas/wyndham-hotels/wyndham-hotels-wp-v2-posts/)
- [Moved to /providers/wyndham-hotels/](https://apis.io/schemas/wyndham-hotels/wyndham-hotels-wp-v2-search/)
- [Moved to /providers/wyndham-hotels/](https://apis.io/schemas/wyndham-hotels/wyndham-hotels-wp-v2-statuses/)
- [Moved to /providers/wyndham-hotels/](https://apis.io/schemas/wyndham-hotels/wyndham-hotels-wp-v2-tags/)
- [Moved to /providers/wyndham-hotels/](https://apis.io/schemas/wyndham-hotels/wyndham-hotels-wp-v2-taxonomies/)
- [Moved to /providers/wyndham-hotels/](https://apis.io/schemas/wyndham-hotels/wyndham-hotels-wp-v2-types/)
- [Moved to /providers/wyndham-hotels/](https://apis.io/schemas/wyndham-hotels/wyndham-hotels-wp-v2-users/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Wyndham Hotels Authentication](https://apis.io/security/wyndham-hotels/wyndham-hotels-authentication/)
- [Wyndham Hotels Domain Security](https://apis.io/security/wyndham-hotels/wyndham-hotels-domain-security/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Wyndham Hotels Scopes](https://apis.io/scopes/wyndham-hotels/wyndham-hotels-scopes/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.wyndhamhotels.com/)
- [Support](https://www.wyndhamhotels.com/contact-us)
- [Blog](https://corporate.wyndhamhotels.com/news-media/)
- [Terms of service](https://www.wyndhamhotels.com/about-us/terms-of-use-more-info)
- [Privacy policy](https://www.wyndhamhotels.com/about-us/privacy-notice-more-info)
- [GitHub](https://github.com/Wyndham-Hotels-Resorts)

## API Evangelist rating

**Kin Score 20.9** — emerging · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 71.7 |
| Contract quality | 0.0 |
| Contract governance | 4.5 |
| Operational transparency | 2.6 |
| Developer ergonomics | 28.6 |
| Access clarity | 21.1 |

**Agent readiness 22.3** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | — |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | platform (partial credit) |
| Auth Clarity | served (partial credit) |
| Idempotency | — |
| Error Semantics | documented (partial credit) |
| OpenAPI Examples | — |
| Rate Limit Signal | — |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | yes |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | served (partial credit) |
| Protected Resource Metadata | verified |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | na |

**Regulatory alignment 34.3** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/wyndham-hotels/](https://apis.io/providers/wyndham-hotels/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Wyndham Hotels & Resorts: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/wyndham-hotels/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
