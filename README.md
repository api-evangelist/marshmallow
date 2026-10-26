# Marshmallow (marshmallow)

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

Marshmallow is a London-headquartered UK insurtech founded in 2017 by twins Alexander and Oliver Kent-Braham with engineer David Goate, built around a single underserved segment: people who have recently moved to the United Kingdom. Traditional UK motor underwriters ignore overseas driving history and price newcomers punitively, so Marshmallow built its own pricing, fraud and underwriting models that consume global rather than only national driving data. It owns the whole value chain rather than renting a carrier's paper — distribution through Marshmallow Financial Services Limited (FCA FRN 797672), car finance through Marshmallow Credit Services Limited (FCA FRN 1024606), and underwriting through Marshmallow Insurance Limited, an authorised insurance undertaking regulated by the Gibraltar Financial Services Commission that files an annual Solvency and Financial Condition Report. Lines of business are private motor and telematics motor, van, home (buildings, contents and personal possessions) and car finance, sold direct-to-consumer through an app and web quote flow, with offices in London and Budapest.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/marshmallow/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/marshmallow/refs/heads/main/apis.yml)

## Tags

- Insurance
- United Kingdom
- Insurtech
- Property and Casualty
- Motor Insurance
- Home Insurance
- Telematics
- Underwriting
- Claims
- Direct to Consumer
- Partner Gated
- No Public API

## Timestamps

- **Created:** 2026-07-25
- **Modified:** 2026-07-25

## APIs

**None.** Marshmallow publishes no public, self-serve API.

Every conventional developer entry point was probed on 2026-07-25:

| Surface | HTTP | Finding |
| --- | --- | --- |
| `developer.marshmallow.com` | — | Does not resolve |
| `developers.marshmallow.com` | — | Does not resolve |
| `sandbox.marshmallow.com` | — | Does not resolve |
| `docs.marshmallow.com` | 403 | CloudFront distribution exists; blocks anonymous callers on every path |
| `api.marshmallow.com` | 403 | Live private nginx API for Marshmallow's own app; no spec, no discovery, no docs |
| `auth.marshmallow.com` | 401 | Real OAuth 2.0 / OIDC authorization server, closed to unregistered clients |
| `marshmallow.com/developers` | 404 | Not present |
| `marshmallow.com/api` | 404 | Not present |
| `marshmallow.com/partners` | 404 | Not present |
| `marshmallow.com/integrations` | 404 | Not present |
| `account.marshmallow.com` | 200 | Consumer account login wall — not a developer portal |

The 369-URL sitemap contains no developer, API, docs, or integration page. There is no public Postman workspace, no GraphQL endpoint, no published `.proto`, no webhook or AsyncAPI catalog, and no SDK. The public GitHub organization [marshmallow-insurance](https://github.com/marshmallow-insurance) holds four repositories — all front-end libraries (`smores-react`, `smores-icons`, `campfire`, `.github`), none of them API artifacts.

None of the four insurance verbs — **quote**, **bind**, **issue**, **FNOL** — is exposed to third parties. All four exist only as consumer web and app journeys served by Marshmallow's private API.

## ACORD posture

**No ACORD reference found.** No mention of ACORD, AL3, ACORD XML, ACORD certification, or NGDS appears anywhere on Marshmallow's public properties. As a UK personal-lines direct writer with an in-house stack and no independent-agency channel, Marshmallow has no agency-download, IVANS, Applied Epic or Vertafore dependency. The absence is structural, not an oversight.

## Auth model

The single anonymously reachable machine-readable artifact Marshmallow serves is its OpenID Connect discovery document, harvested verbatim to [`well-known/marshmallow-openid-configuration.json`](well-known/marshmallow-openid-configuration.json):

- **Issuer:** `https://auth.marshmallow.com`
- **Grants:** `authorization_code`, `client_credentials`, `refresh_token`, `urn:ietf:params:oauth:grant-type:token-exchange`
- **Client auth:** `client_secret_basic`, `client_secret_post`, `client_secret_jwt`, `private_key_jwt`, `tls_client_auth`, `self_signed_tls_client_auth`
- **PKCE:** `S256` · **mTLS:** yes · **certificate-bound access tokens:** yes · **DPoP:** yes
- **Scopes published:** `openid` only

That is a capable authorization server — the profile of an operator that integrates with regulated financial counterparties. But no product scopes are published, there is no dynamic client registration, and nothing documents how a third party would obtain a client. The infrastructure for partner integration exists; the public developer programme does not.

## Why this is the expected outcome

The United Kingdom has the FCA and PRA but **no open-insurance obligation**. Unlike Open Banking, no rule compels a UK insurer to expose quote, policy, claims, or customer-data APIs, and the FCA's Open Finance work remains consultation rather than rule. The one market-wide API and data modernization effort in UK insurance is the London Market's Blueprint Two / PPL / Whitespace / Ki programme — aimed at brokers and syndicates in the subscription market, invisible from the outside, and irrelevant to a personal-lines direct writer. Marshmallow's zero public API surface is market behaviour, not a laggard signal.

## Artifacts

Enrichment round 2026-07-25. Everything below was searched, probed, or derived from what Marshmallow actually publishes — nothing is inferred from a spec, because there is no spec.

| Artifact | File | Method | What it holds |
| --- | --- | --- | --- |
| Well-known index | [`well-known/marshmallow-well-known.yml`](well-known/marshmallow-well-known.yml) | searched | Every `/.well-known/` path probed on all five Marshmallow hosts with its HTTP status. One hit (OIDC discovery); no RFC 9116 `security.txt` anywhere. `account.marshmallow.com` returns 200 for every path but the body is the SPA HTML shell, recorded as `html-shell`, not a hit. |
| Authentication | [`authentication/marshmallow-authentication.yml`](authentication/marshmallow-authentication.yml) | searched | The OIDC profile: endpoints, four grant types, six client-auth methods, PKCE S256, mTLS + certificate-bound tokens, DPoP, no dynamic client registration. |
| OAuth scopes | [`scopes/marshmallow-scopes.yml`](scopes/marshmallow-scopes.yml) | searched | The single published scope, `openid`. Zero product scopes. |
| Conformance | [`conformance/marshmallow-conformance.yml`](conformance/marshmallow-conformance.yml) | derived | OAuth/OIDC RFC conformance read off the discovery document (7636, 7009, 7523, 7662, 8693, 8705, 9449 all yes; 7591 and 8414 no), plus explicit `false` on OpenAPI, AsyncAPI, ACORD and security.txt, `unknown` where there is nothing to inspect, and the FCA/GFSC regulatory register. |
| Domain security | [`security/marshmallow-domain-security.yml`](security/marshmallow-domain-security.yml) | probed | TLS 1.3 on all five hosts; HSTS only on `auth.` and `account.`; no CAA, no DNSSEC; SPF present, DMARC `p=reject`. |
| Packages | [`packages/marshmallow-packages.yml`](packages/marshmallow-packages.yml) | searched | Three first-party npm packages under `@mrshmllw`. **Zero API client SDKs** — eight registries probed. |
| Components | [`components/marshmallow-components.yml`](components/marshmallow-components.yml) | searched | The public "Smores" front-end estate (React components, design tokens, archived icons, Campfire utils). No embeddable third-party quote/policy/claims surface. |
| llms.txt | [`llms/marshmallow-llms.txt`](llms/marshmallow-llms.txt) | generated | Agent-readable summary of this repo; `https://www.marshmallow.com/llms.txt` returns 404. |

No `openapi/`, `asyncapi/`, `mcp/`, `skills/`, `arazzo/`, `errors/`, `conventions/`, `sandbox/`, `changelog/`, `cli/`, `lifecycle/` or `grpc/` artifacts exist here, and none were fabricated: each requires a machine-readable contract or a documentation host that Marshmallow does not expose. `status.`, `trust.`, `partners.`, `developers.` and `mcp.` subdomains do not resolve; there is no public Postman workspace; the org `SECURITY.md` is GitHub's unmodified template with no contact, so no vulnerability-disclosure artifact was recorded.

## Links

- [Website](https://www.marshmallow.com/)
- [Our story](https://www.marshmallow.com/our-story)
- [Blog](https://www.marshmallow.com/blog)
- [Claims](https://www.marshmallow.com/claims)
- [Help centre](https://www.marshmallow.com/help)
- [Solvency and Financial Condition Reports](https://www.marshmallow.com/solvency-and-financial-condition-report)
- [GitHub](https://github.com/marshmallow-insurance)
- [LinkedIn](https://www.linkedin.com/company/marshmallowltd)
- [Review findings](review.yml)

> **Homonym note:** the widely used Python `marshmallow` serialization library ([marshmallow-code](https://github.com/marshmallow-code)) is unrelated to this company.
