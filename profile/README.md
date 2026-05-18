# Groupsum

Groupsum builds governed developer systems for teams that need source-controlled truth, traceable delivery, and reusable operations.

Our public work focuses on two connected surfaces:

- [ssot-registry](https://github.com/groupsum/ssot-registry) is a portable single-source-of-truth system for features, claims, tests, evidence, ADRs, specs, frozen boundaries, and releases.
- [markdown_workspace](https://github.com/groupsum/markdown_workspace) is the MdWrk workspace for markdown applications, native shells, extension contracts, distribution tooling, repository governance, and release automation.

## What We Build

Groupsum projects are designed around explicit records, reproducible checks, and durable repository workflows. The goal is simple: decisions, implementation scope, verification, and release state should be discoverable from the repo instead of scattered across chat, documents, and build logs.

## Public Projects

### ssot-registry

`ssot-registry` provides a canonical `.ssot/registry.json` model plus CLI and Python surfaces for managing governed delivery records. It tracks features, tests, claims, evidence, issues, risks, ADRs, specs, boundaries, and releases as linked entities.

Use it when you need:

- a repository-native registry for product and engineering scope
- traceable links from decisions to specs, features, tests, evidence, and releases
- CLI-first workflows for validation, upgrades, graph exports, and certification gates
- portable governance that can be adopted by different repositories without rewriting the operating model

Start here:

```bash
python -m pip install ssot-registry
ssot --help
ssot-registry init . --repo-id repo:example --repo-name "Example" --version 0.1.0
ssot-registry validate . --write-report
```

### Governance Packs

Groupsum publishes installable SSOT Registry governance packs for teams that want reusable ADR and SPEC starting points without copying policy language by hand. Each pack is packaged as a Python project, supports Python 3.10 through 3.14, and is designed to synchronize reusable ADR/SPEC assets into downstream `.ssot` registries.

#### Discovery And Content Governance

- [seo-aeo-aieo-governance-pack](https://github.com/groupsum/seo-aeo-aieo-governance-pack) supplies governed SEO, AEO, and AiEO decision/specification templates for search, answer-engine, and AI-engine optimization work.
- [cache-freshness-governance-pack](https://github.com/groupsum/cache-freshness-governance-pack) supplies HTTP caching and freshness governance templates for cache-control, ETag, CDN, invalidation, and stale-content policy surfaces.

#### Trust, Signature, And Records Governance

- [digital-signature-governance-pack](https://github.com/groupsum/digital-signature-governance-pack) supplies digital-signature, electronic-signature, timestamping, validation, archival, and assurance-language governance templates.
- [privacy-governance-records-governance-pack](https://github.com/groupsum/privacy-governance-records-governance-pack) supplies privacy governance record templates for notices, lawful basis, consent records, data subject rights, retention, privacy evidence, and regulatory accountability.
- [data-catalog-lineage-contracts-governance-pack](https://github.com/groupsum/data-catalog-lineage-contracts-governance-pack) supplies data catalog and lineage contract templates for dataset ownership, field definitions, lineage records, transformation provenance, data quality, and evidence retention.

#### Digital Analytics And Behavioral Telemetry

- [web-app-analytics-governance-pack](https://github.com/groupsum/web-app-analytics-governance-pack) supplies web and app analytics templates for page views, screen views, sessions, engagement, ecommerce, data layers, client/server collection, and export validation.
- [web-performance-rum-governance-pack](https://github.com/groupsum/web-performance-rum-governance-pack) supplies web performance and RUM templates for Core Web Vitals, Navigation Timing, Resource Timing, long tasks, performance observers, and real-user measurement evidence.
- [event-behavioral-telemetry-governance-pack](https://github.com/groupsum/event-behavioral-telemetry-governance-pack) supplies event and behavioral telemetry templates for event naming, payload contracts, user actions, session context, timestamps, identifiers, and validation evidence.
- [ga4-google-tagging-governance-pack](https://github.com/groupsum/ga4-google-tagging-governance-pack) supplies GA4 and Google tagging templates for event models, recommended events, parameters, Google tag deployment, consent mode, ecommerce events, and export expectations.

#### Marketing Attribution And Advertising Measurement

- [url-query-attribution-foundations-governance-pack](https://github.com/groupsum/url-query-attribution-foundations-governance-pack) supplies URL query attribution templates for UTM parameters, query parsing, canonical campaign fields, redirect handling, referrer interaction, and attribution evidence.
- [marketing-attribution-conversion-governance-pack](https://github.com/groupsum/marketing-attribution-conversion-governance-pack) supplies marketing attribution and conversion templates for campaign identifiers, conversion events, attribution windows, deduplication, offline conversions, and reporting controls.
- [mobile-install-attribution-governance-pack](https://github.com/groupsum/mobile-install-attribution-governance-pack) supplies mobile install attribution templates for app install measurement, SKAdNetwork, Android attribution, deferred deep links, campaign parameters, and privacy-preserving attribution.
- [ad-measurement-media-governance-pack](https://github.com/groupsum/ad-measurement-media-governance-pack) supplies advertising and media measurement templates for OpenRTB, AdCOM, VAST, OMID, IAB measurement guidance, MRC controls, invalid traffic, and reporting policy.
- [ad-supply-chain-transparency-governance-pack](https://github.com/groupsum/ad-supply-chain-transparency-governance-pack) supplies supply-chain transparency templates for ads.txt, app-ads.txt, sellers.json, SupplyChain Object, buyers.json, DemandChain Object, and ads.cert.

#### Customer, Commerce, Identity, And Consent

- [customer-identity-profile-governance-pack](https://github.com/groupsum/customer-identity-profile-governance-pack) supplies customer identity and profile templates for identifier governance, profile stitching, resolution policy, account linking, consent-aware identity use, and profile lifecycle controls.
- [customer-commerce-semantics-governance-pack](https://github.com/groupsum/customer-commerce-semantics-governance-pack) supplies customer and commerce semantics templates for schema.org, GS1 identifiers, product entities, offer metadata, order events, and retail/customer data modeling.
- [consent-privacy-signals-governance-pack](https://github.com/groupsum/consent-privacy-signals-governance-pack) supplies consent and privacy signal templates for GPC, TCF, consent mode, opt-out handling, privacy preference propagation, and jurisdiction-aware collection controls.
- [audience-data-transparency-governance-pack](https://github.com/groupsum/audience-data-transparency-governance-pack) supplies audience-data transparency templates for IAB data transparency, audience taxonomy, content taxonomy, segment provenance, recency, permitted use, and clean-room outputs.
- [gs1-product-link-event-data-governance-pack](https://github.com/groupsum/gs1-product-link-event-data-governance-pack) supplies GS1 product link and event data templates for Digital Link, product identifiers, EPCIS-style event data, supply-chain context, and traceability records.

### markdown_workspace

`markdown_workspace` contains MdWrk, a multi-package markdown platform covering web client delivery, native app shells, reusable packages, extension contracts, first-party extensions, third-party extension distribution tooling, and repository operations.

Use it when you need:

- governed markdown application infrastructure
- Electron and Capacitor shell delivery
- extension runtime contracts and distribution tooling
- repository conformance checks for docs, release notes, generated artifacts, and claim language

Start here:

```bash
npm run ci:governance
```

## Operating Principles

- Repositories should carry their own decisions, specs, scope, verification, and release evidence.
- Automation should read from durable files and typed records before relying on informal process.
- Public docs should give humans and machines direct answers, stable links, and concrete commands.
- Governance should make delivery clearer, not heavier.

## Links

- Organization: [github.com/groupsum](https://github.com/groupsum)
- SSOT registry: [github.com/groupsum/ssot-registry](https://github.com/groupsum/ssot-registry)
- Governance packs:
  [discovery and content](https://github.com/groupsum/seo-aeo-aieo-governance-pack),
  [cache freshness](https://github.com/groupsum/cache-freshness-governance-pack),
  [digital signature](https://github.com/groupsum/digital-signature-governance-pack),
  [privacy records](https://github.com/groupsum/privacy-governance-records-governance-pack),
  [data catalog lineage](https://github.com/groupsum/data-catalog-lineage-contracts-governance-pack),
  [web app analytics](https://github.com/groupsum/web-app-analytics-governance-pack),
  [web performance RUM](https://github.com/groupsum/web-performance-rum-governance-pack),
  [event behavioral telemetry](https://github.com/groupsum/event-behavioral-telemetry-governance-pack),
  [GA4 Google tagging](https://github.com/groupsum/ga4-google-tagging-governance-pack),
  [URL query attribution](https://github.com/groupsum/url-query-attribution-foundations-governance-pack),
  [marketing attribution conversion](https://github.com/groupsum/marketing-attribution-conversion-governance-pack),
  [mobile install attribution](https://github.com/groupsum/mobile-install-attribution-governance-pack),
  [ad measurement media](https://github.com/groupsum/ad-measurement-media-governance-pack),
  [ad supply chain transparency](https://github.com/groupsum/ad-supply-chain-transparency-governance-pack),
  [customer identity profile](https://github.com/groupsum/customer-identity-profile-governance-pack),
  [customer commerce semantics](https://github.com/groupsum/customer-commerce-semantics-governance-pack),
  [consent privacy signals](https://github.com/groupsum/consent-privacy-signals-governance-pack),
  [audience data transparency](https://github.com/groupsum/audience-data-transparency-governance-pack), and
  [GS1 product link event data](https://github.com/groupsum/gs1-product-link-event-data-governance-pack)
- MdWrk workspace: [github.com/groupsum/markdown_workspace](https://github.com/groupsum/markdown_workspace)
