# Mews (mews-com)

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

Mews is a cloud-native hospitality operating system serving 15,000+ hotels, hostels, and vacation-rental properties across 85 countries. Founded in Prague in 2012 by Richard Valtr and Matthijs Welle and reaching unicorn status in 2024, Mews offers an integrated Property Management System, Point of Sale, Revenue Management, embedded Payments, Booking Engine, and a Marketplace of 1,000+ third-party apps. The Mews Open API surface — Connector, Booking Engine, Distributor, Channel Manager, POS, and Loyalty Partner APIs — handles 10M+ messages per day and is the integration backbone for the modern hotel tech stack.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/mews-com/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/mews-com/refs/heads/main/apis.yml)

## Scope

- **Position:** Producing
- **Access:** 3rd-Party

## Tags

- Hospitality
- Hotel
- PMS
- Property Management
- Travel
- Booking
- Reservations
- Cloud
- SaaS

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### Mews Connector API

General-purpose API that gives partners of Mews access to data and services in Mews Operations. Covers reservations, customers, companies, accounting, bills, payments, rates and availability, products and services, enterprises and resources, cashiers and counters, exports, loyalty memberships, devices and printers, customer messaging, billing automations, vouchers, restrictions, and resource access tokens. JSON-over-HTTPS request/response with `ClientToken` + `AccessToken` authentication; 197 operations across ~30 resource groups; webhooks delivered as API Events.

- **Human URL:** [https://docs.mews.com/connector-api](https://docs.mews.com/connector-api)
- **Base URL:** `https://api.mews.com/api/connector/v1`

#### Tags

- Hospitality
- Hotel
- PMS
- Property Management
- Reservations
- Connector

#### Properties

- [Documentation](https://docs.mews.com/connector-api)
- [Documentation](https://docs.mews.com/connector-api/guidelines)
- [Documentation](https://docs.mews.com/connector-api/concepts)
- [Documentation](https://docs.mews.com/connector-api/operations)
- [Webhooks](https://docs.mews.com/connector-api/api-events)
- [OpenAPI](https://api.mews.com/Swagger/connector/swagger.yaml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [OpenAPI](openapi/mews-connector-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mews-connector-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mews-connector-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/mews-reservation-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/mews-customer-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/mews-com-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### Mews Booking Engine API

Web API for booking engines and booking widgets to interact programmatically with Mews — fetch offered rooms and spaces, check availability and pricing, retrieve products and promotions, authorize payment cards, and create reservation groups. Covers services, restrictions, exchange rates, payment configuration, and reservation pricing for a single property.

- **Human URL:** [https://docs.mews.com/booking-engine-guide/booking-engine-api](https://docs.mews.com/booking-engine-guide/booking-engine-api)
- **Base URL:** `https://api.mews.com/api/bookingEngine/v1`

#### Tags

- Hospitality
- Hotel
- Booking Engine
- Reservations
- Direct Bookings

#### Properties

- [Documentation](https://docs.mews.com/booking-engine-guide/booking-engine-api)
- [OpenAPI](https://api.mews.com/Swagger/bookingEngine/swagger.yaml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [OpenAPI](openapi/mews-booking-engine-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mews-booking-engine-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mews-booking-engine-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Mews Distributor API

Legacy/distribution surface used by the Mews-hosted booking widget. Retrieves hotel info, availability and pricing, language/currency/country reference data, payment configuration, voucher validation, exchange rates, and reservation creation. Same JSON-over-HTTPS shape and token auth as the Connector API.

- **Human URL:** [https://docs.mews.com/distributor-api](https://docs.mews.com/distributor-api)
- **Base URL:** `https://api.mews.com/api/distributor/v1`

#### Tags

- Hospitality
- Hotel
- Booking
- Distribution
- Direct Bookings

#### Properties

- [Documentation](https://docs.mews.com/distributor-api)
- [OpenAPI](https://api.mews.com/Swagger/distributor/swagger.yaml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [OpenAPI](openapi/mews-distributor-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mews-distributor-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mews-distributor-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Mews Channel Manager API

Two-way API for channel managers and distribution channels. Mews-side operations let channel managers receive reservations from Mews; channel-manager-side endpoints let Mews push availability, rate, and inventory updates outbound. Mediates OTA, GDS, and metasearch traffic into the Mews reservation graph.

- **Human URL:** [https://docs.mews.com/channel-manager-api](https://docs.mews.com/channel-manager-api)

#### Tags

- Hospitality
- Hotel
- Channel Manager
- Distribution
- Inventory

#### Properties

- [Documentation](https://docs.mews.com/channel-manager-api)
- [Documentation](https://docs.mews.com/channel-manager-api/usage-guidelines)
- [Documentation](https://docs.mews.com/channel-manager-api/concepts)
- [Changelog](https://docs.mews.com/channel-manager-api/changelog)
- [Postman Collection](collections/mews-booking-engine-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mews-booking-engine-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/mews-connector-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mews-connector-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/mews-distributor-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mews-distributor-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Mews POS API

API for Point-of-Sale systems to integrate with Mews — provides real-time visibility into F&B operations including outlets, items, orders, and invoices, and pushes charges onto guest bills inside the Mews PMS. Used by partner POS vendors and Mews POS itself.

- **Human URL:** [https://docs.mews.com/pos-api](https://docs.mews.com/pos-api)

#### Tags

- Hospitality
- Hotel
- POS
- Point of Sale
- Food and Beverage

#### Properties

- [Documentation](https://docs.mews.com/pos-api)
- [Postman Collection](collections/mews-booking-engine-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mews-booking-engine-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/mews-connector-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mews-connector-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/mews-distributor-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mews-distributor-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Mews Loyalty Partner API

Reverse API for loyalty program providers — Mews calls the partner's endpoints to look up members, validate enrollment, fetch tier and benefit data, and record earn/redeem activity during the guest journey. Complements the Connector API Loyalty operation group on the Mews side.

- **Human URL:** [https://docs.mews.com/loyalty-partner-api](https://docs.mews.com/loyalty-partner-api)

#### Tags

- Hospitality
- Hotel
- Loyalty
- Members
- Rewards

#### Properties

- [Documentation](https://docs.mews.com/loyalty-partner-api)
- [Postman Collection](collections/mews-booking-engine-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mews-booking-engine-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/mews-connector-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mews-connector-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/mews-distributor-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mews-distributor-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Arazzo Workflows](arazzo/) — [Arazzo Specification](https://spec.openapis.org/arazzo/latest.html)
- [Portal](https://www.mews.com/)
- [Documentation](https://docs.mews.com/)
- [Documentation](https://www.mews.com/en/products/api)
- [Documentation](https://docs.mews.com/connector-api/getting-started)
- [GitHub Organization](https://github.com/MewsSystems)
- [Documentation](https://github.com/MewsSystems/open-api-docs)
- [Marketplace](https://www.mews.com/en/marketplace)
- [Sign Up](https://www.mews.com/en/partnerships)
- [Support](https://help.mews.com/)
- [Forum](https://community.mews.com/)
- [Blog](https://www.mews.com/en/blog)
- [Status Page](https://status.mews.com/)
- [Pricing](https://www.mews.com/en/pricing)
- [Terms of Service](https://www.mews.com/en/terms-conditions/partners)
- [Privacy Policy](https://www.mews.com/en/privacy-policy)
- [Trust Center](https://trust.mews.com/)
- [Webhooks](https://docs.mews.com/connector-api/api-events)
- [Rate Limits](https://docs.mews.com/connector-api/guidelines)
- [Errors](https://docs.mews.com/connector-api/guidelines)
- [Versioning](https://docs.mews.com/connector-api/changelog)
- [Changelog](https://docs.mews.com/connector-api/changelog)
- [SDK](https://github.com/MewsSystems/fiscalizations)
- [SDK](https://github.com/MewsSystems/mews-flutter)
- [Code Examples](https://github.com/MewsSystems/awesome-mews)
- [Tool](https://github.com/MewsSystems/developers)
- [LinkedIn](https://www.linkedin.com/company/mews-systems/)
- [X (Twitter)](https://x.com/mewssystems)
- [YouTube](https://www.youtube.com/@MewsSystems)
- [Careers](https://www.mews.com/en/careers)
- [Plans](plans/mews-com-plans-pricing.yml)
- [Rate Limits](rate-limits/mews-com-rate-limits.yml)
- [Fin Ops](finops/mews-com-finops.yml)
- [Vocabulary](vocabulary/mews-com-vocabulary.yml)
- [Spectral Rules](rules/mews-com-rules.yml)
- [Features](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
**URL:** https://apievangelist.com
