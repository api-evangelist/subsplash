# Subsplash (subsplash)

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

Subsplash is an all-in-one church and ministry engagement platform - custom mobile and TV apps, websites, media hosting and delivery, online giving, and church management (People, Groups, Events, Volunteers). Subsplash publishes a REST developer API for programmatic access to media, giving records, people, groups and messaging, and event registrations.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/subsplash/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/subsplash/refs/heads/main/apis.yml)

## Access Model (Important)

The Subsplash API is **real but gated**:

- **Documentation is form-gated.** Full developer documentation is released only after submitting the documentation-access form at [developer.subsplash.com/form](https://developer.subsplash.com/form). Subsplash is explicit that "this form grants access to documentation and resources only. It does not provide API credentials."
- **Credentials are rep-provisioned.** API access requires OAuth 2.0 credentials (a Client ID and Client Secret) that must be set up in coordination with a Subsplash representative / Client Success Manager, and generally requires a qualifying paid plan (Pro / Enterprise tier).
- **Authentication is OAuth 2.0.** Public integration material shows OAuth flows (Authorization Code, Client Credentials, and others) with a redirect handled at `https://core.subsplash.com/end-user-auth/v1/authproviders/result`, confirming `core.subsplash.com` as the platform API host.

Because the fully documented endpoint surface sits behind that gate, the APIs described in `apis.yml` are **modeled** (`endpointsModeled: true`) from Subsplash's public product, support, and integration material - not transcribed from an open reference. No `openapi/`, `rate-limits/`, `finops/`, or `collections/` artifacts are published here because no authoritative open specification is available to source them from.

## Tags

- Church
- Ministry
- Nonprofit
- Giving
- Media
- Church Management
- ChMS
- Mobile Apps
- Partner API

## Timestamps

- **Created:** 2026-07-03
- **Modified:** 2026-07-03

## APIs (Modeled)

### Subsplash Media Library API

Programmatic access to an organization's media catalog - sermons, series, podcasts, blogs, and announcements - for syncing content into external sites, AI/search pipelines, and custom apps.

- **Human URL:** [https://developer.subsplash.com/](https://developer.subsplash.com/)
- **Base URL:** `https://core.subsplash.com`

### Subsplash Giving API

Sync online giving and donation records from Subsplash Giving into accounting, CRM, and church-management systems - donations, donors, funds, and recurring gifts.

- **Human URL:** [https://developer.subsplash.com/](https://developer.subsplash.com/)
- **Base URL:** `https://core.subsplash.com`

### Subsplash People API

People Sync surface for unifying member and contact records across systems, plus Single Sign-On (SSO) user provisioning.

- **Human URL:** [https://developer.subsplash.com/](https://developer.subsplash.com/)
- **Base URL:** `https://core.subsplash.com`

### Subsplash Groups and Messaging API

Manage groups, group membership, and messaging, and trigger push notifications and in-app messages through Subsplash's communications engine.

- **Human URL:** [https://developer.subsplash.com/](https://developer.subsplash.com/)
- **Base URL:** `https://core.subsplash.com`

### Subsplash Events API

Manage events, event registrations, and event payments for syncing sign-ups and transactions into external systems.

- **Human URL:** [https://developer.subsplash.com/](https://developer.subsplash.com/)
- **Base URL:** `https://core.subsplash.com`

## Common Properties

- [GitHub Organization](https://github.com/Subsplash)
- [LinkedIn](https://www.linkedin.com/company/subsplash)
- [Website](https://www.subsplash.com)
- [Documentation](https://developer.subsplash.com/)
- [Sign Up (Docs Access Form)](https://developer.subsplash.com/form)
- [Plans](plans/subsplash-plans-pricing.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
