# SimpleLegal

SimpleLegal is Onit's mid-market enterprise legal management (ELM) platform trusted by 550+ corporate legal departments. It provides matter management, eBilling, spend management, vendor management, legal requests, and legal operations analytics for in-house legal teams. The SimpleLegal API is organized around REST with predictable, resource-oriented URLs, enabling integration with ERP and finance systems to eliminate duplicate data entry and automate legal operations workflows.

**Website:** https://www.simplelegal.com/  
**API Documentation:** https://developer.simplelegal.com/  
**Parent Company:** https://www.onit.com/products/elm/simplelegal/  
**GitHub:** https://github.com/SimpleLegal  

## API

### SimpleLegal REST API

The SimpleLegal API is organized around REST with predictable, resource-oriented URLs. HTTP Basic authentication is used. All responses return JSON. The API supports PATCH for partial updates (POST also accepted). Pagination defaults to 25 items per page, configurable via `page_size` query parameter.

**Base URL:** `https://app.simplelegal.com/api/v1`  
**Authentication:** HTTP Basic  

**Key Resources:**
- `/matters` — Create, retrieve, and update legal matters
- `/invoices` — Submit and process legal invoices (eBilling)
- `/vendors` — Manage outside counsel and service providers
- `/cost-codes` — List billing and cost codes (UTBMS, GL codes)
- `/users` — Create and manage platform users
- `/payments` — Record invoice payments for AP/ERP sync

**Key Capabilities:**
- Create matters, invoices, vendors, users, and payments
- Retrieve lists of matters, invoices, cost codes, and more
- Update matter status, invoice approval, and vendor info
- Integrate with AP/ERP systems to eliminate duplicate data entry
- Track legal spend, budgets, and accruals per matter

## Artifacts

### OpenAPI

| Spec | Description |
|---|---|
| [simplelegal-openapi.yml](openapi/simplelegal-openapi.yml) | SimpleLegal REST API — matters, invoices, vendors, cost codes, users, payments |

### Rules

| Ruleset | Description |
|---|---|
| [simplelegal-rules.yml](rules/simplelegal-rules.yml) | Spectral ruleset enforcing SimpleLegal API conventions |

### Capabilities

| Capability | Description |
|---|---|
| [legal-operations-management.yaml](capabilities/legal-operations-management.yaml) | Unified legal operations management workflow — matters, invoices, vendors, spend, users |

**Shared Definitions:**

| Shared File | Description |
|---|---|
| [shared/simplelegal.yaml](capabilities/shared/simplelegal.yaml) | SimpleLegal API consumed definition |

### JSON Schema

| Schema | Description |
|---|---|
| [simplelegal-matter-schema.json](json-schema/simplelegal-matter-schema.json) | Legal matter schema |
| [simplelegal-invoice-schema.json](json-schema/simplelegal-invoice-schema.json) | Legal invoice schema |
| [simplelegal-vendor-schema.json](json-schema/simplelegal-vendor-schema.json) | Vendor schema |

### JSON Structure

| Structure | Description |
|---|---|
| [simplelegal-matter-structure.json](json-structure/simplelegal-matter-structure.json) | Matter field documentation |
| [simplelegal-invoice-structure.json](json-structure/simplelegal-invoice-structure.json) | Invoice field documentation |

### JSON-LD

| Context | Description |
|---|---|
| [simplelegal-context.jsonld](json-ld/simplelegal-context.jsonld) | SimpleLegal legal operations vocabulary linked data context |

### Examples

| Example | Description |
|---|---|
| [simplelegal-create-matter-example.json](examples/simplelegal-create-matter-example.json) | Create a new legal matter |
| [simplelegal-list-invoices-example.json](examples/simplelegal-list-invoices-example.json) | List pending invoices for a matter |
| [simplelegal-create-vendor-example.json](examples/simplelegal-create-vendor-example.json) | Create a new outside counsel vendor |

### Vocabulary

| Vocabulary | Description |
|---|---|
| [simplelegal-vocabulary.yml](vocabulary/simplelegal-vocabulary.yml) | SimpleLegal domain vocabulary covering matter management, eBilling, spend management, vendor relations, and legal operations |

## Common Properties

| Property | URL |
|---|---|
| Website | https://www.simplelegal.com/ |
| API Documentation | https://developer.simplelegal.com/ |
| Blog | https://www.simplelegal.com/blog/ |
| Parent Company | https://www.onit.com/products/elm/simplelegal/ |
| GitHub | https://github.com/SimpleLegal |
| Support | https://support.simplelegal.com/ |
| CounselGO Vendor Portal | https://www.simplelegal.com/counselgo |
| Legal Requests | https://info.simplelegal.com/legal-requests-datasheet |

## Tags

eBilling, Enterprise Legal Management, Legal Operations, Legal Spend Management, Matter Management, Vendor Management

## Maintainers

- Kin Lane (kin@apievangelist.com)
