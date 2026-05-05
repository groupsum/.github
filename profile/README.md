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
- MdWrk workspace: [github.com/groupsum/markdown_workspace](https://github.com/groupsum/markdown_workspace)
