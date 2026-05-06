# Standards & API Reference

> Project: Fitness Studio Management · Generated: 2026-05-03

## Industry Standards & Specifications

### ISO Standards

**ISO/IEC 27001:2022 — Information Security Management**
- URL: https://www.iso.org/standard/27001
- Relevance: Establishes requirements for an information security management system (ISMS). Fitness studio management platforms handling member personal data, payment credentials, and health information should target ISO 27001 certification as a baseline trust signal for enterprise clients and franchise operators.

**ISO/IEC 27018:2019 — Protection of Personally Identifiable Information in Public Clouds**
- URL: https://www.iso.org/standard/76559.html
- Relevance: Supplements ISO 27001 with controls for cloud-hosted SaaS products that process PII. Directly applicable to any fitness platform storing member profiles, billing history, and health/attendance data in multi-tenant cloud infrastructure.

**ISO 9241 — Ergonomics of Human-System Interaction**
- URL: https://www.iso.org/standard/77520.html
- Relevance: Provides internationally recognised guidelines on usability, interaction design, and ergonomics for software interfaces. Relevant to both the studio operator admin console and member-facing mobile app to ensure learnability and efficiency for non-technical users.

---

### W3C & IETF Standards

**RFC 5545 — Internet Calendaring and Scheduling Core Object Specification (iCalendar)**
- URL: https://www.rfc-editor.org/rfc/rfc5545
- Relevance: The foundational standard for representing and exchanging calendaring events, to-dos, and free/busy information. Fitness studio class schedules exported or synced to member calendars (Google Calendar, Apple Calendar, Outlook) must conform to RFC 5545 for interoperability.

**RFC 7265 — jCal: The JSON Format for iCalendar**
- URL: https://www.rfc-editor.org/rfc/rfc7265.html
- Relevance: Defines a JSON-native encoding of the RFC 5545 data model. Useful for REST API responses that include class schedule or booking event data, enabling roundtrip conversion between iCalendar and JSON without semantic loss.

**RFC 5546 — iCalendar Transport-Independent Interoperability Protocol (iTIP)**
- URL: https://datatracker.ietf.org/doc/html/rfc5546
- Relevance: Specifies the protocol and constraints for scheduling event interchange between calendar systems, including meeting invitations and responses. Relevant for studio-to-member class booking confirmation and cancellation notification flows.

**RFC 6749 — The OAuth 2.0 Authorization Framework**
- URL: https://www.rfc-editor.org/rfc/rfc6749
- Relevance: The standard for delegated authorisation used by all major fitness platforms (Mindbody, Pike13, Vagaro, Wodify) to secure their APIs. Any third-party integration with a fitness studio platform must implement OAuth 2.0 flows.

**RFC 8252 — OAuth 2.0 for Native Apps**
- URL: https://datatracker.ietf.org/doc/html/rfc8252
- Relevance: Defines best practices for OAuth 2.0 on native mobile apps (iOS, Android). Critical for the member mobile app component, which must use external user-agents (system browser) for auth flows rather than embedded web views.

**RFC 7636 — PKCE (Proof Key for Code Exchange)**
- URL: https://datatracker.ietf.org/doc/html/rfc7636
- Relevance: Extends OAuth 2.0 with PKCE, which is now mandatory for all public clients (mobile apps, SPAs). Prevents authorisation code interception attacks in mobile app authentication flows.

**OpenID Connect Core 1.0**
- URL: https://openid.net/specs/openid-connect-core-1_0.html
- Relevance: Identity layer on top of OAuth 2.0 enabling member sign-in with existing identity providers (Google, Apple, Facebook). Enables "Sign in with Google/Apple" flows on the member app without building a custom identity system.

**WCAG 2.2 — Web Content Accessibility Guidelines**
- URL: https://www.w3.org/WAI/standards-guidelines/wcag/
- Relevance: W3C accessibility standard referenced in ADA Title III enforcement and required by many enterprise clients. Member booking flows, admin dashboards, and mobile apps should target WCAG 2.2 Level AA compliance to meet ADA obligations and serve members with disabilities.

---

### Data Model & API Specifications

**OpenAPI Specification 3.1 (OAS 3.1)**
- URL: https://spec.openapis.org/oas/v3.1.1.html
- Relevance: Industry-standard interface description language for REST APIs. All major fitness studio platforms with public APIs (Mindbody, Pike13, Vagaro, Wodify, TeamUp) should expose OpenAPI 3.1 specs for tooling, SDK generation, and documentation. Fully compatible with JSON Schema Draft 2020-12.

**JSON Schema Draft 2020-12**
- URL: https://json-schema.org/specification
- Relevance: The standard for describing and validating JSON data structures. Used to define fitness data models (Member, ClassSession, Booking, Membership, Payment) in API request/response bodies and for validating webhook payloads.

**HL7 FHIR R4 — Fast Healthcare Interoperability Resources**
- URL: https://hl7.org/fhir/R4/
- Relevance: The de facto standard for health data exchange. Relevant when fitness platforms expose workout, biometric, or attendance data to third-party wellness platforms, insurance programmes, or healthcare providers. FHIR `Observation` resources can represent workout performance, heart rate, and body composition data from wearables.

---

### Security & Authentication Standards

**PCI DSS v4.0 — Payment Card Industry Data Security Standard**
- URL: https://www.pcisecuritystandards.org/document_library/
- Relevance: Mandatory for any platform processing, transmitting, or storing credit/debit card data. All membership billing, POS transactions, and retail purchases on a fitness studio platform are in scope. Compliance requires encryption, access controls, network segmentation, and regular security assessments.

**GDPR — General Data Protection Regulation (EU) 2016/679**
- URL: https://gdpr-info.eu/
- Relevance: Applies to any fitness platform serving European members or operating in the EU. Governs collection, storage, and processing of member PII (name, email, health data, payment history). Requires explicit consent, data subject rights (access, deletion, portability), and data processing agreements.

**CCPA — California Consumer Privacy Act**
- URL: https://oag.ca.gov/privacy/ccpa
- Relevance: California privacy law granting consumers rights over personal data. Fitness studios serving California members must honour opt-out of data sale, right to deletion, and right to know what data is collected. Similar state laws are expanding across the US.

**HIPAA — Health Insurance Portability and Accountability Act**
- URL: https://www.hhs.gov/hipaa/
- Relevance: HIPAA applies when a fitness platform handles Protected Health Information (PHI), such as medical condition details used to tailor programming, injury records, or data shared with healthcare providers. While most fitness studios are not covered entities, platforms offering health-adjacent features (rehabilitation, medical fitness) must evaluate HIPAA applicability carefully.

**OWASP Application Security Verification Standard (ASVS)**
- URL: https://owasp.org/www-project-application-security-verification-standard/
- Relevance: A framework of security requirements for web and mobile application development. Relevant to API authentication, session management, data validation, and error handling in fitness platform development. ASVS Level 2 is appropriate for platforms handling payment and health data.

---

### MCP Server Specifications

**Model Context Protocol (MCP)**
- URL: https://modelcontextprotocol.io/
- Relevance: Anthropic's open standard for connecting AI models to external tools and data sources. Relevant for an AI-native fitness studio management platform exposing member data, class schedules, and analytics to LLM agents for churn prediction, programme generation, and automated communications. An MCP server interface could allow AI assistants to read booking data, member profiles, and retention signals without custom integrations.

---

## Similar Products — Developer Documentation & APIs

### Mindbody

- **Description:** The largest fitness and wellness management platform, serving mid-to-large studios, gyms, and spas. Provides class scheduling, membership billing, marketing, and a consumer-facing discovery marketplace.
- **API Documentation:** https://developers.mindbodyonline.com/ui/documentation/public-api
- **API Release Notes:** https://developers.mindbodyonline.com/Resources/ApiReleaseNotes
- **Developer Portal:** https://developers.mindbodyonline.com/
- **SDKs/Libraries:** No official SDKs; community-maintained wrappers exist on GitHub for Python and Node.js.
- **Standards:** REST/JSON. Public API with key-based and OAuth authentication. OpenAPI spec not publicly published.
- **Authentication:** API key + site ID for public endpoints; OAuth 2.0 for user-level access.

---

### Vagaro

- **Description:** An all-in-one platform for fitness studios, salons, and spas covering scheduling, POS, payroll, and a consumer marketplace. Strong among small-to-mid studios.
- **API Documentation:** https://docs.vagaro.com/public/docs/introduction
- **Webhook Documentation:** https://docs.vagaro.com/public/docs/webhook-events
- **Developer Support:** https://support.vagaro.com/hc/en-us/categories/34949493949851-Developer-Features
- **SDKs/Libraries:** No official SDKs listed. REST/JSON API accessible via API key.
- **Standards:** REST/JSON. Webhooks via HTTPS POST with JSON payload. OAuth not required for basic API access.
- **Authentication:** API key. Webhooks require HTTPS endpoint returning 2xx within 20 seconds.

---

### Pike13

- **Description:** Cloud-based business management software for fitness studios, dance schools, and multi-activity facilities. Known for its clean API and strong developer support relative to its market size.
- **API Documentation:** https://developer.pike13.com/docs/api/v2
- **Developer Center:** https://developer.pike13.com/
- **Getting Started Guide:** https://developer.pike13.com/docs/get_started
- **SDKs/Libraries:** No official SDKs; API is well-documented for custom integration development.
- **Standards:** REST/JSON. Three APIs: Core API (business operations), Reporting API (analytics aggregation), Webhooks API (event notifications). OpenAPI 2.x spec partially available.
- **Authentication:** OAuth 2.0 (authorisation code flow).

---

### Zen Planner (Daxko)

- **Description:** Membership management platform for martial arts schools, CrossFit gyms, and functional fitness studios. Acquired by Daxko; now part of a broader health/wellness software portfolio.
- **API Documentation:** https://docs.partners.daxko.com/openapi/ZenPlanner/v1/
- **SDKs/Libraries:** No official SDKs.
- **Standards:** REST/JSON with OpenAPI spec published via Daxko partner portal.
- **Authentication:** API key via partner programme; OAuth 2.0 for partner-level access.

---

### Wodify

- **Description:** Gym management platform built for CrossFit affiliates, functional fitness gyms, jiu-jitsu schools, and boutique studios. Unique strength in workout tracking, performance leaderboards, and the digital whiteboard feature.
- **API Documentation:** https://docs.wodify.com/docs/getting-started
- **Program API:** https://help.wodify.com/hc/en-us/articles/209425797-Wodify-s-Program-API
- **API Tracker Entry:** https://apitracker.io/a/wodify
- **SDKs/Libraries:** No official SDKs; REST API documented at docs.wodify.com (updated March 2026).
- **Standards:** REST/JSON. API covers clients, leads, classes, memberships, and performance data.
- **Authentication:** API key for basic access; OAuth 2.0 for partner integrations.

---

### TeamUp

- **Description:** Fitness and gym management software serving independent studios and regional multi-location groups. Praised for transparent pricing, flexible membership configuration, and a genuinely open API at no additional cost.
- **API Documentation:** https://goteamup.com/features/teamup-api
- **API Base URL:** https://api.goteamup.com/
- **SDKs/Libraries:** No official SDKs; all plans include API access and credentials.
- **Standards:** REST/JSON. Zapier integration available for no-code automation. API access included in all plans at no extra cost.
- **Authentication:** API key generated via account settings.

---

### Hapana

- **Description:** AI-native fitness studio management platform with white-label member apps, engagement analytics, challenge/reward gamification, and 40+ partner integrations. Targets growth-stage boutique brands and multi-site operators.
- **API Documentation:** Not publicly listed; available to partners via the Hapana integrations directory.
- **Integrations Directory:** https://www.hapana.com/integrations
- **SDKs/Libraries:** No public SDKs identified. Platform claims 40+ integrations via open API.
- **Standards:** REST/JSON assumed; specific API schema not publicly documented.
- **Authentication:** API key / partner access; specific OAuth details not published.

---

### Glofox (ABC Fitness)

- **Description:** Boutique fitness studio management platform with white-label apps, member lifecycle analytics, and retention-focused tooling. Now operating under ABC Fitness following acquisition.
- **API Documentation:** https://apitracker.io/a/glofox (community tracker)
- **SDKs/Libraries:** No official public SDKs.
- **Standards:** REST/JSON. Integration via partner programme with webhook support.
- **Authentication:** OAuth 2.0 for partner integrations; API key for direct access (via partner agreement).

---

## Notes

**Emerging area — wearable data standards**: There is growing demand for fitness platforms to ingest data from wearables (Apple Watch, Garmin, Polar, Fitbit/Google). No single standard dominates; most integrations use proprietary vendor APIs (Apple HealthKit, Google Fit / Health Connect, Garmin Connect API, Polar AccessLink API). HL7 FHIR is gaining traction for health-system-adjacent fitness data exchange but is not yet widely implemented in commercial studio management platforms.

**API maturity gap**: Many fitness studio platforms (Hapana, Glofox) do not publish full OpenAPI specs or developer documentation publicly — integrations require commercial partnership agreements. This is a significant barrier for open-source or AI-native tools seeking to interoperate with the ecosystem. Pike13 and TeamUp have the most accessible public APIs among the surveyed tools.

**Spot Booking trademark**: The term "Spot Scheduling®" is a registered trademark of Zingfit/Mariana Tek. Any new platform implementing equipment-selection booking should use distinct terminology (e.g., "seat reservation", "equipment booking", "position selection") to avoid infringement risk.

**MCP opportunity**: No current fitness studio platform exposes an MCP server interface. This represents a clean differentiation opportunity for an AI-native tool — enabling LLM agents to directly query member data, retention signals, and class schedules without custom integration work.
