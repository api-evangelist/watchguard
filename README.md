# WatchGuard

WatchGuard provides cloud-managed network and endpoint security solutions including Firebox next-generation firewalls, WatchGuard Endpoint Security (WES), AuthPoint multi-factor authentication, and WatchGuard Wi-Fi. WatchGuard Cloud is the unified management platform exposing RESTful APIs for account management, device activation, asset allocation, endpoint device management, security event monitoring, and operator administration.

**Website:** https://www.watchguard.com  
**API Documentation:** https://www.watchguard.com/help/docs/API/  
**Developer Portal:** https://developer.cloud.watchguard.com/  
**Getting Started:** https://www.watchguard.com/help/docs/API/Content/en-US/api_get_started/get_started.html  
**APIs.json:** https://raw.githubusercontent.com/api-evangelist/watchguard/refs/heads/main/apis.yml

## Tags

Cloud Security, Endpoint Security, Firewall, MFA, Network Security, Zero Trust

---

## APIs

### WatchGuard Cloud Platform API

RESTful API for managing WatchGuard Cloud accounts, sub-accounts, and operators. Covers account creation, audience token generation for managed account access, hardware/license activation, asset allocation, and operator management.

- **Documentation:** https://www.watchguard.com/help/docs/API/Content/en-US/watchguard-cloud/watchguard-cloud.html
- **OpenAPI:** [openapi/watchguard-cloud-platform-openapi.yml](openapi/watchguard-cloud-platform-openapi.yml)

**Key endpoints:** Accounts, Authorization (Audience), Activations, Allocations, Operators

### WatchGuard Endpoint Security Management API

RESTful API for managing WatchGuard Endpoint Security (WES) devices. Covers device listing, protection status, network isolation, immediate scans, security events, security overviews, and risk assessment.

- **Documentation:** https://www.watchguard.com/help/docs/API/Content/en-US/endpoint_security/WES_endpoint_security/v1/WES_endpoint_security.html
- **OpenAPI:** [openapi/watchguard-endpoint-security-openapi.yml](openapi/watchguard-endpoint-security-openapi.yml)

**Key endpoints:** Devices, Protection Status, Isolation, Immediate Scan, Security Events, Security Overview, Risk Assessment, Configurations, Licenses

---

## Artifacts

### OpenAPI Specifications

| File | Description |
|------|-------------|
| [openapi/watchguard-cloud-platform-openapi.yml](openapi/watchguard-cloud-platform-openapi.yml) | Platform API — accounts, activation, allocation, operators |
| [openapi/watchguard-endpoint-security-openapi.yml](openapi/watchguard-endpoint-security-openapi.yml) | Endpoint Security API — device management, events, risk |

### Spectral Rules

| File | Description |
|------|-------------|
| [rules/watchguard-rules.yml](rules/watchguard-rules.yml) | Spectral ruleset enforcing dual security schemes, account ID requirements, HTTPS, Title Case summaries |

### Naftiko Capabilities

| File | Description |
|------|-------------|
| [capabilities/endpoint-threat-response.yaml](capabilities/endpoint-threat-response.yaml) | Endpoint Threat Response workflow — 14 MCP tools for device management, isolation, scanning, and risk review |
| [capabilities/shared/cloud-platform.yaml](capabilities/shared/cloud-platform.yaml) | Shared Platform API — account, activation, operator operations |
| [capabilities/shared/endpoint-security.yaml](capabilities/shared/endpoint-security.yaml) | Shared Endpoint Security API — device and event operations |

### JSON Schemas

| File | Description |
|------|-------------|
| [json-schema/watchguard-device-schema.json](json-schema/watchguard-device-schema.json) | Endpoint device schema with protection status and isolation fields |

### JSON Structures

| File | Description |
|------|-------------|
| [json-structure/watchguard-device-structure.json](json-structure/watchguard-device-structure.json) | Endpoint device field structure documentation |

### JSON-LD Contexts

| File | Description |
|------|-------------|
| [json-ld/watchguard-context.jsonld](json-ld/watchguard-context.jsonld) | JSON-LD context for WatchGuard data vocabulary |

### Examples

| File | Description |
|------|-------------|
| [examples/watchguard-getAccount-example.json](examples/watchguard-getAccount-example.json) | Get Account Information request/response |
| [examples/watchguard-listDevices-example.json](examples/watchguard-listDevices-example.json) | List Endpoint Devices request/response |
| [examples/watchguard-isolateDevices-example.json](examples/watchguard-isolateDevices-example.json) | Isolate Devices request/response |
| [examples/watchguard-activateDevice-example.json](examples/watchguard-activateDevice-example.json) | Activate Device or License request/response |

### Vocabulary

| File | Description |
|------|-------------|
| [vocabulary/watchguard-vocabulary.yml](vocabulary/watchguard-vocabulary.yml) | Domain vocabulary: WatchGuard Cloud, Account, Firebox, Device Isolation, Activation, Allocation, ThreatSync, AuthPoint |

---

## Maintainers

**FN:** Kin Lane  
**Email:** kin@apievangelist.com
