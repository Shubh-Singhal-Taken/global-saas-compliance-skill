---
name: global-saas-compliance
description: Assess product-level SaaS compliance across jurisdictions. Use when building, reviewing, launching, or changing web, mobile, API, or AI software. Determine applicability first, separate laws from standards, map requirements to engineering controls and evidence, and verify current authoritative sources.
---

# Global SaaS Compliance Skill

Use this skill for product/software compliance, not company formation, tax, payroll, accounting, or founder registration.

## Core rules
- This is compliance-engineering guidance, not legal advice.
- Never claim legal compliance from a checklist alone.
- Determine applicability from territorial scope, thresholds, roles, data, features, customers, and dates.
- Separate legal requirements, conditional regulations, contractual/customer requirements, and voluntary standards.
- For current law, verify authoritative primary sources and record source date/effective date.
- If facts or law are uncertain, say so; never invent requirements.

## Workflow
1. Build a product profile: product type, users, countries, customers, features, data categories, data subjects, processing roles, hosting/processing locations, transfers, retention, payments, security, AI models/providers, and sector.
2. Determine served and potentially triggered jurisdictions.
3. Identify triggers: personal/sensitive data, children, employment, education, profiling/automated decisions, AI, UGC/intermediary activity, ads/tracking, payments, cross-border transfers, public-sector use, regulated sectors, accessibility, IP/open source, incident reporting.
4. Build an applicability matrix for every candidate requirement.
5. Prioritise: P0 legal/launch blocker; P1 legal/high risk; P2 conditional/customer-critical; P3 voluntary hardening; N/A assessed non-applicable.
6. Map each requirement to engineering controls.
7. Map controls to evidence.
8. Re-verify P0/P1 requirements, effective dates, vendors, notices, and material AI/profiling changes before release.

## Compliance record
Record: requirement_id, jurisdiction, instrument, category, applies (yes/no/conditional/unknown), trigger, product_scope, effective_date, enforcement_date, source_url, source_checked_at, authority, confidence, rationale, controls, evidence, owner, status, and notes.

## Global domains
PRIVACY_DATA_PROTECTION; CYBERSECURITY; AI_GOVERNANCE; COOKIES_TRACKING; MARKETING_COMMUNICATIONS; ACCESSIBILITY; PAYMENTS_CARD_DATA; CONSUMER_SAAS; PLATFORM_INTERMEDIARY; INTELLECTUAL_PROPERTY; OPEN_SOURCE; SECURITY_ASSURANCE; BUSINESS_CONTINUITY; SECTOR_HEALTH; SECTOR_FINANCE; SECTOR_INSURANCE; SECTOR_EDUCATION; SECTOR_EMPLOYMENT; GOVERNMENT_PUBLIC_SECTOR.

## Candidate jurisdiction frameworks
- India: DPDP Act/Rules, IT Act, CERT-In, applicable IT Rules.
- EU/EEA: GDPR, ePrivacy, DSA, European Accessibility Act, EU AI Act.
- UK: UK GDPR, Data Protection Act 2018, PECR.
- US: CCPA/CPRA, state privacy laws, FTC Act, COPPA, CAN-SPAM, TCPA, sector laws.
- Canada: PIPEDA and provincial privacy laws.
- Australia: Privacy Act and APPs.
- Singapore: PDPA.
- Japan: APPI.
- South Korea: PIPA.
- China: PIPL, Data Security Law, Cybersecurity Law.
- Brazil: LGPD.
- South Africa: POPIA.
- UAE: applicable federal personal-data framework plus free-zone/sector rules.
- Saudi Arabia: PDPL and implementing rules.

These are candidate frameworks, not automatic applicability conclusions.

## Standards (track separately from law)
ISO/IEC 27001; ISO/IEC 27701; ISO/IEC 27017; ISO/IEC 27018; ISO/IEC 42001; ISO 22301; SOC 2; NIST CSF; NIST AI RMF; OWASP ASVS; PCI DSS; WCAG.

## Engineering examples
- Data rights: request intake, identity verification, access/export/correct/delete, audit trail.
- Retention: retention classes, deletion jobs, backup expiry, legal holds.
- Consent: purpose-specific records, versioned notices, withdrawal and propagation.
- Security: MFA, RBAC, encryption, secrets management, logging, monitoring, incident response, backups.
- AI: model inventory, risk classification, data-use controls, human oversight, transparency, evaluation, model/version logging.
- Cookies: tracker inventory, consent, logging, opt-out, preferences.

## Special product triggers
Recruitment AI: assess profiling/automated decisions, fairness, human review, candidate rights, resume retention and scraping/source terms.
Developer/hackathon platforms: minimise OAuth scopes, log repository access, enforce tenant isolation, define code retention/deletion, protect secrets and review API/IP terms.
Payments: determine whether raw card data enters the boundary; prefer hosted/tokenised payment collection; determine PCI DSS scope.

## Agent portability
Do not require vendor-specific tools. An agent may use web search, browser, repository files, local scripts, user documents, or compliance databases. Without web access, use bundled references and mark freshness-sensitive conclusions needs-verification.

## Output modes
DISCOVERY; APPLICABILITY; CHECKLIST; ENGINEERING; AUDIT; CHANGE_IMPACT; LAUNCH_GATE; REPORT.
Default: APPLICABILITY + CHECKLIST + ENGINEERING.

## Final sections
Confirmed applicable; Conditional / needs facts; Not applicable based on current facts; Needs legal verification; Engineering actions; Evidence to collect.
