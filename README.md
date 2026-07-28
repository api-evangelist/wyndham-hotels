# Wyndham Hotels & Resorts (wyndham-hotels)

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

No APIs are documented for Wyndham Hotels & Resorts.

The `developer.`, `developers.`, `docs.` and `api.` subdomains of `wyndhamhotels.com` do not resolve. `/developers`, `/api`, `/docs`, `/openapi.json`, `/swagger.json`, `/api-docs` and `/.well-known/` all return 404. An `mcp.wyndhamhotels.com` host exists in certificate transparency and resolves, but every path returns an Akamai 503 with no served content and no documentation — it is recorded as an observation in `review.yml`, not catalogued as an API.

The programmable interface to Wyndham inventory belongs to Sabre Hospitality, whose SynXis Central Reservation System Wyndham buys, not to Wyndham. See `review.yml` for the full probe log and the switching-cost analysis.

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
