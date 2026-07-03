# Subsplash (subsplash)

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
