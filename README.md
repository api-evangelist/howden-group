# Howden Group (howden-group)

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
