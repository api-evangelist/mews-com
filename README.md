# Mews (mews-com)

Mews is a cloud-native hospitality operating system serving 15,000+ hotels, hostels, and vacation-rental properties across 85 countries. Founded in Prague in 2012 by Richard Valtr and Matthijs Welle and reaching unicorn status in 2024, Mews offers an integrated Property Management System, Point of Sale, Revenue Management, embedded Payments, Booking Engine, and a Marketplace of 1,000+ third-party apps. The Mews Open API surface — Connector, Booking Engine, Distributor, Channel Manager, POS, and Loyalty Partner APIs — handles 10M+ messages per day and is the integration backbone for the modern hotel tech stack.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/mews-com/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

 - Hospitality, Hotel, PMS, Property Management, Travel, Booking, Reservations, Cloud, SaaS

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## Open API Surface

| API | Style | Base URL | Notes |
|---|---|---|---|
| Connector API | JSON-over-HTTPS POST (RPC) | `https://api.mews.com/api/connector/v1/` | 197 operations across ~30 resource groups |
| Booking Engine API | JSON-over-HTTPS POST | `https://api.mews.com/api/bookingEngine/v1/` | Direct-booking widget backend |
| Distributor API | JSON-over-HTTPS POST | `https://api.mews.com/api/distributor/v1/` | Legacy Mews-hosted booking widget |
| Channel Manager API | Two-way JSON-over-HTTPS | n/a (negotiated) | OTA / GDS / metasearch distribution |
| POS API | JSON-over-HTTPS POST | `https://api.mews.com/api/pos/v1/` | F&B Point-of-Sale integration |
| Loyalty Partner API | Reverse webhook | Partner-hosted | Mews calls the loyalty provider |

Production environment: `https://api.mews.com`. Demo / sandbox: `https://api.mews-demo.com`.

## APIs

### Mews Connector API
General-purpose API that gives partners of Mews access to data and services in Mews Operations. Covers reservations, customers, companies, accounting, bills, rates and availability, products and services, enterprises and resources, cashiers and counters, exports, loyalty memberships, devices and printers, customer messaging, billing automations, vouchers, restrictions, and resource access tokens. 197 operations.

**Human URL:** [https://docs.mews.com/connector-api](https://docs.mews.com/connector-api)

- [Documentation](https://docs.mews.com/connector-api)
- [Usage Guidelines](https://docs.mews.com/connector-api/guidelines)
- [Concepts](https://docs.mews.com/connector-api/concepts)
- [API Operations](https://docs.mews.com/connector-api/operations)
- [API Events (Webhooks)](https://docs.mews.com/connector-api/api-events)
- [OpenAPI](openapi/mews-connector-api-openapi.yml)
- [JSON Schema — Reservation](json-schema/mews-reservation-schema.json)
- [JSON Schema — Customer](json-schema/mews-customer-schema.json)
- [JSON-LD Context](json-ld/mews-com-context.jsonld)
- [Naftiko Capability — Reservations](capabilities/connector-reservations.yaml)
- [Naftiko Capability — Customers](capabilities/connector-customers.yaml)
- [Naftiko Capability — Availability and Rates](capabilities/connector-availability.yaml)
- [Naftiko Capability — Bills, Payments, Accounting](capabilities/connector-bills.yaml)
- [Naftiko Capability — Webhooks](capabilities/connector-webhooks.yaml)

### Mews Booking Engine API
Web API for booking engines and booking widgets — fetch offered rooms and spaces, check availability and pricing, retrieve products and promotions, authorize payment cards, and create reservation groups.

**Human URL:** [https://docs.mews.com/booking-engine-guide/booking-engine-api](https://docs.mews.com/booking-engine-guide/booking-engine-api)

- [OpenAPI](openapi/mews-booking-engine-api-openapi.yml)
- [Naftiko Capability — Reservations](capabilities/booking-engine-reservations.yaml)
- [Naftiko Capability — Availability and Pricing](capabilities/booking-engine-availability.yaml)

### Mews Distributor API
Legacy/distribution surface used by the Mews-hosted booking widget. Hotel info, availability and pricing, language/currency/country reference data, payment configuration, voucher validation, exchange rates, and reservation creation.

**Human URL:** [https://docs.mews.com/distributor-api](https://docs.mews.com/distributor-api)

- [OpenAPI](openapi/mews-distributor-api-openapi.yml)
- [Naftiko Capability — Availability](capabilities/distributor-availability.yaml)

### Mews Channel Manager API
Two-way API for channel managers and distribution channels. Mews-side endpoints accept reservations from channel managers; channel-manager-side endpoints accept availability, rate, and inventory pushes from Mews.

**Human URL:** [https://docs.mews.com/channel-manager-api](https://docs.mews.com/channel-manager-api)

### Mews POS API
API for Point-of-Sale partners. Outlets, items, orders, invoices, and bill posting from F&B systems into the Mews PMS.

**Human URL:** [https://docs.mews.com/pos-api](https://docs.mews.com/pos-api)

### Mews Loyalty Partner API
Reverse API for loyalty program providers — Mews calls the partner's endpoints to look up members, validate enrollment, fetch tier and benefit data, and record earn/redeem activity.

**Human URL:** [https://docs.mews.com/loyalty-partner-api](https://docs.mews.com/loyalty-partner-api)

## Commercial

- [Plans & Pricing (reconciled)](plans/mews-com-plans-pricing.yml) — three named tiers (Essentials, Professional, Enterprise) plus Mews Payments and Marketplace Partner program; all quote-based.
- [Rate Limits (reconciled)](rate-limits/mews-com-rate-limits.yml) — per-partner concurrency, per-endpoint throttling, cursor-pagination guidance, webhook-first guidance.
- [FinOps (FOCUS-aligned)](finops/mews-com-finops.yml) — subscription + payment-transaction billing surface.

## Schema and Tooling

- [Spectral Ruleset](rules/mews-com-rules.yml)
- [Vocabulary](vocabulary/mews-com-vocabulary.yml)
- [JSON Structure — Reservation domain](json-structure/mews-com-reservation-structure.json)
- Examples:
  - [Connector reservations/getAll](examples/mews-connector-reservations-getall-example.json)
  - [Booking Engine services/getAvailability](examples/mews-booking-engine-availability-example.json)

## Common Resources

- [Mews Open API Docs](https://docs.mews.com/)
- [Mews Open API Product Page](https://www.mews.com/en/products/api)
- [Mews Marketplace](https://www.mews.com/en/marketplace)
- [Mews Help Center](https://help.mews.com/)
- [Mews Community](https://community.mews.com/)
- [Status Page](https://status.mews.com/)
- [Trust Center](https://trust.mews.com/)
- [Partner Program](https://www.mews.com/en/partnerships)
- [GitHub — MewsSystems](https://github.com/MewsSystems)
- [Mews Flutter SDK](https://github.com/MewsSystems/mews-flutter)
- [Mews Fiscalizations .NET library](https://github.com/MewsSystems/fiscalizations)
- [Awesome Mews](https://github.com/MewsSystems/awesome-mews)

## Company

- Founded: 2012 in Prague
- Founders: Richard Valtr, Matthijs Welle (CEO)
- HQ: Prague (with offices in London and the US)
- Scale: 15,000+ properties across 85 countries; 1,300+ employees
- Funding: Unicorn ($1B+ valuation, 2024); Series D raise in 2026
- Certifications: SOC 2, ISO 27001, PCI DSS
