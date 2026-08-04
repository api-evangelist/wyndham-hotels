# Wyndham Hotels & Resorts (wyndham-hotels)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Wyndham Hotels & Resorts, Inc. (NYSE: WH) is the world's largest hotel franchising company by number of properties, with over 8,300 affiliated hotels and approximately 869,000 rooms across roughly 25 brands in 95+ countries, licensed to more than 6,200 franchisees. Headquartered in Parsippany, New Jersey, its home market is the United States. Wyndham does not operate most of its hotels — it franchises brands (Days Inn, Super 8, Ramada, La Quinta, Microtel, Baymont, Howard Johnson, Travelodge, Wingate, Wyndham, Wyndham Grand, Trademark Collection, TRYP, Dolce, ECHO Suites and others) and sells the demand that flows through them. It sits in the distribution chain as a franchisor and demand aggregator rather than as a distribution platform: inventory reaches buyers through Wyndham's own brand.com sites and Wyndham Rewards, through GDS chain codes under master chain code WR, and through third-party online travel agents, with the central reservation layer supplied by Sabre Hospitality's SynXis CRS. Its API posture is thin and honest: as of 2026-07-28 there is no developer portal, no API documentation, no OpenAPI or other machine-readable contract, and no public API terms — and the published Terms of Use affirmatively prohibit robots, spiders, meta-searching and automated access to its AI Search.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/wyndham-hotels/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/wyndham-hotels/refs/heads/main/apis.yml)

## Tags

- Travel
- United States
- Hospitality
- Hotels
- Booking
- Franchising
- Distribution
- Loyalty
- GDS

## Timestamps

- **Created:** 2026-07-28
- **Modified:** 2026-07-28

## APIs

**No APIs are documented for Wyndham Hotels & Resorts** — but three undocumented, live machine-readable surfaces were found and are catalogued honestly:

- **Wyndham Business WordPress REST API** — `https://www.wyndhambusiness.com/wp-json/wp/v2` — anonymous, 309 registered routes across 12 namespaces, JSON Schema available by HTTP OPTIONS. Incidental CMS infrastructure, not a product.
- **Wyndham Business WordPress MCP Server (OAuth-gated)** — `https://www.wyndhambusiness.com/wp-json/mcp/mcp-oauth-server` — a real OAuth 2.1 protected resource with RFC 8414 and RFC 9728 discovery metadata, PKCE S256 and a single `mcp` scope. Anonymous `tools/list` returns 401 with a standards-correct bearer challenge; no tool list is readable and no client registration path is published.
- **Wyndham Hotel Development WordPress REST API** — `https://development.wyndhamhotels.com/wp-json/wp/v2` — anonymous, 403 routes across 17 namespaces, plus a third (non-OAuth) MCP adapter that returns 401.

None of these carries hotel data. There is no property, rate, availability, reservation, loyalty or folio entity in any machine-readable Wyndham surface, and no OpenAPI, AsyncAPI, GraphQL, webhook or SDK anywhere.

The `developer.`, `developers.`, `docs.` and `api.` subdomains of `wyndhamhotels.com` do not resolve. `/developers`, `/api`, `/docs`, `/openapi.json`, `/swagger.json`, `/api-docs` and `/.well-known/` all return 404 on the consumer estate. An `mcp.wyndhamhotels.com` host exists in certificate transparency and resolves, but every path returns an Akamai 503 with no served content and no documentation — it is recorded as an observation in `review.yml`, not catalogued as an API.

Wyndham's stated posture and its deployed posture disagree: the Terms of Use effective 2026-03-12 prohibit robots, spiders, intelligent agents and meta-searching outright, while three MCP adapters run on the estate.

The programmable interface to Wyndham inventory belongs to Sabre Hospitality, whose SynXis Central Reservation System Wyndham buys, not to Wyndham. See `review.yml` for the full probe log, the round-two correction, and the switching-cost analysis.

## Switching Cost

- **Interface shape:** `none-published` — no standard reference found; no OpenTravel/OTA, HTNG, OpenAPI or NDC conformance claim anywhere public.
- **Second source:** `alternatives-with-migration` — for a franchisee, Choice, Best Western, G6, Sonesta, IHG and independence all exist, but exiting a "typically 10 to 20 years in length" franchise agreement plus reflagging is a capital project.
- **Exit path:** `export-on-request` — the Privacy Notice publishes a real data-portability right, exercised by email, phone or mail only. No bulk export operation, no business-data export.
- **Identifier portability:** GDS chain codes (master chain **WR**; e.g. **WG** Wingate) and IATA/ARC agency numbers travel; Wyndham Rewards member numbers and Wyndham Direct 10-digit corporate codes do not.
- **Contractual lock-in:** 10-to-20-year franchise terms, ~5% royalty plus a 2-4% marketing and reservation fee on gross room revenue, a Wyndham-installed PMS amortized over "the remaining non-cancellable period of the franchise agreement", and a Terms of Use banning automated access that "terminate automatically if you fail to comply with any provision hereof".
- **Distribution model:** `gds-intermediated` — Wyndham's own travel-agent material says a rate is "bookable through the GDS only".
- **NDC posture:** Not applicable (hotel group, not an airline).
- **Access gate:** `none-published` — nothing to sign up for, because nothing is offered.

## Common Properties

- [Website](https://www.wyndhamhotels.com/)
- [Corporate Website](https://corporate.wyndhamhotels.com/)
- [LinkedIn](https://www.linkedin.com/company/wyndhamhotels)
- [Wikipedia](https://en.wikipedia.org/wiki/Wyndham_Hotels_%26_Resorts)
- [Terms of Service](https://www.wyndhamhotels.com/about-us/terms-of-use-more-info)
- [Privacy Policy](https://www.wyndhamhotels.com/about-us/privacy-notice-more-info)
- [llms.txt](https://www.wyndhamhotels.com/llms.txt)
- [robots.txt](https://www.wyndhamhotels.com/robots.txt)
- [Sitemap](https://www.wyndhamhotels.com/sitemap.xml)
- [Investor Relations](https://investor.wyndhamhotels.com/)
- [FY2025 Form 10-K](https://www.sec.gov/Archives/edgar/data/1722684/000172268426000007/wh-20251231.htm)
- [Wyndham Hotel Development (Franchising)](https://development.wyndhamhotels.com/)
- [Wyndham Supplier Portal](https://wyndham.supplierone.co/)
- [Wyndham Hotel Travel Advisors Program](https://www.wyndhamhotels.com/content/whg-ecomm-responsive/en-us/whg/about-us/travel-professionals.html)
- [Wyndham Business](https://www.wyndhambusiness.com/)
- [Wyndham Rewards](https://www.wyndhamhotels.com/wyndham-rewards)
- [GitHub Organization](https://github.com/Wyndham-Hotels-Resorts)
- [Predecessor: Wyndham Worldwide](https://raw.githubusercontent.com/api-evangelist/wyndham-worldwide/refs/heads/main/apis.yml)
- [Review](review.yml)

## Maintainers

- Kin Lane — kin@apievangelist.com
