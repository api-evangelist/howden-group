# Howden Group (howden-group)

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

Howden Group Holdings is a London-headquartered, employee-owned international insurance intermediary founded in 1994, operating across retail insurance broking (Howden), specialty and reinsurance broking (Howden Re / Howden Specialty), and managing general agency underwriting (DUAL). Its home market is the United Kingdom and the Lloyd's of London subscription market, with lines of business spanning property and casualty, specialty, credit and political risk, marine, cyber, employee benefits, and reinsurance.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/howden-group/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/howden-group/refs/heads/main/apis.yml)

## Tags

- Insurance
- United Kingdom
- Broker
- Insurance Broking
- Reinsurance
- Specialty Insurance
- Managing General Agent
- Employee Benefits
- Credit Insurance
- London Market
- ACORD
- Partner Gated

## Timestamps

- **Created:** 2026-07-25
- **Modified:** 2026-07-25

## APIs

**None.** Howden Group publishes no public, self-serve API and no downloadable API definition. This is the honest and expected outcome for a UK broker-intermediary: the United Kingdom has an FCA and a PRA but no open-insurance obligation, and the FCA's Open Finance work remains consultation rather than rule.

Probed on 2026-07-25:

| Surface | Result |
| --- | --- |
| `developer.howdengroup.com` | DNS does not resolve |
| `developers.howdengroup.com` | DNS does not resolve |
| `docs.howdengroup.com` | DNS does not resolve |
| `api.howdengroup.com` | DNS does not resolve |
| `howdengroup.com/developers` | 404 |
| `howdengroup.com/api` | 404 |
| `howdengroup.com/developer` | 404 |
| `howdengroup.com/partners` | 404 |
| `howdengroup.com/integrations` | 404 |
| `parentportal.howdengroup.com` | 200 — login wall, "Howden Insurance Portal" |
| `tepfinx.com` | 200 — partner placement application shell, no docs |
| `developer.dualinsurance.com` | 200 — cPanel placeholder, parked host |

No OpenAPI, Swagger, AsyncAPI, Postman collection, GraphQL schema, or `.proto` file was found. Every `/openapi.json`, `/swagger.json` and `/api-docs` probe that returned 200 served an HTML soft-404 shell.

## What Howden actually integrates

The integration work is real — it is simply bilateral and invisible from the outside.

- **ACORD GRLC digital accounting and invoicing, live.** On 3 July 2025 ACORD and Howden announced that ACORD Standards for digital accounting and invoicing are live and operational in the UK retail insurance market — the first use of ACORD digital accounting standards in the UK outside the specialty and (re)insurance market. Howden operationalised the ACORD GRLC (Global Reinsurance & Large Commercial) Standards using ACORD Solutions Group's **ADEPT** (ACORD Data Exchange Platform & Translator) as a messaging gateway and portal, with retail insurer partner **Hiscox**. ADEPT is cloud-native and supports both XML and JSON messaging over API architecture.
- **HowdenCAP / Tepfin X direct carrier APIs.** HowdenCAP markets itself as "the only broker in the London structured credit insurance market to have direct APIs with insurers," connecting its Tepfin X placement application to carrier underwriting platforms one partner at a time — Allianz Trade (October 2022), AXA XL, and Mosaic Insurance. These carry presentation, negotiation, binding and management of credit insurance contracts. Partner-only, contracted, undocumented publicly.
- **London market modernization.** Howden (RKH Specialty) participated in Lloyd's closed Beta Group refining the Core Data Record under **Blueprint Two**, and partnered with **Whitespace** for digital placement. Blueprint Two, PPL and Whitespace are market infrastructure aimed at brokers and syndicates, not developers — which is precisely why the UK's best insurance API work stays invisible from outside.

## Insurance API verbs

| Verb | Exposure |
| --- | --- |
| Quote | Partner-only (Tepfin X submission intake and triage) |
| Bind | Partner-only (bilateral carrier APIs) |
| Issue | Partner-only (contract management; accounting via ACORD GRLC over ADEPT) |
| FNOL / Claims | Not exposed — no claims API surface found |

## Auth model

Not publicly documented, because no public API exists. Observable surfaces are browser login walls. No OIDC or OAuth authorization-server metadata is served at `/.well-known/openid-configuration` or `/.well-known/oauth-authorization-server` on any Howden host probed. Partner API credentials for the Tepfin X and ADEPT integrations are issued under bilateral contract.

## Links

- [Website](https://www.howdengroup.com/uk-en)
- [About Howden](https://www.howdengroup.com/uk-en/about-us)
- [Howden Insurance Portal (login)](https://parentportal.howdengroup.com/)
- [LinkedIn](https://www.linkedin.com/company/howden-broking-insurance)
- [ACORD and Howden pioneer digital invoicing standards in the UK retail market](https://www.acord.org/ACORD-about/acord-news/2025/07/03/acord-and-howden-pioneer-the-adoption-of-digital-invoicing-standards-in-the-uk-retail-insurance-market)
- [Howden CAP and AXA XL collaborate to develop structured credit APIs](https://www.howdengroup.com/news-and-insights/howden-cap-and-axa-xl-collaborate-to-develop-structured-credit-apis)
- [Howden and Allianz Trade partner on API connectivity](https://www.howdengroup.com/news-and-insights/Howden-and-Allianz-Trade-partner-on-API-connectivity)

## Review

See [review.yml](review.yml) for the full API Evangelist reviewer finding, every probe with its HTTP status, and the ACORD posture in detail.
