<!-- @format -->

# `.github` (`Xernerx/.github`) — Agent Guidelines (`AGENTS.md`)

## 🧭 Overview

`d:\Xernerx Studios\.github` (`github.com/Xernerx/.github`) is the **GitHub Organization profile and community health repository** for **Xernerx Studios**. All repositories in the `Xernerx` organization (`suite`, `virtue`, `docs`, `xernerx`, `framework`, `commands`, `extension-builder`, `hooks`, `stats`, `terminal`, `websocket`) inherit their default community standards and issue/PR templates from this repository.

## 🗂️ Canonical Files

- [`profile/README.md`](./profile/README.md): Public organization profile rendered on `github.com/Xernerx`.
- [`README.md`](./README.md): Repository overview and GitHub UI surface map.
- [`CODE_OF_CONDUCT.md`](./CODE_OF_CONDUCT.md): Inherited Contributor Covenant v2.1 Code of Conduct.
- [`CONTRIBUTING.md`](./CONTRIBUTING.md): Inherited contribution guide covering both Tier 1 (`Xernerx Proprietary & SaaS License v1.0`) and Tier 2 (`Apache-2.0` open-source SDKs).
- [`SECURITY.md`](./SECURITY.md): Inherited security policy, supported versions table, and vulnerability disclosure guidelines (`security@xernerx.com` / `xernerx.com/security`).
- [`SUPPORT.md`](./SUPPORT.md): Inherited support routing banner for New Issue / PR views.
- [`FUNDING.yml`](./FUNDING.yml): Organization sponsor links (`store.xernerx.com`, `xernerx.com`).
- [`PULL_REQUEST_TEMPLATE.md`](./PULL_REQUEST_TEMPLATE.md) & [`ISSUE_TEMPLATE/`](./ISSUE_TEMPLATE): Default PR checklist and YAML issue forms (`bug_report.yml`, `feature_request.yml`, `config.yml`).
- [`LICENSE`](./LICENSE): `Apache-2.0` license.

## ⚠️ Important Rules

1. **No Shadowing in Sibling Repositories:** Do not create duplicate `SECURITY.md`, `CODE_OF_CONDUCT.md`, or `CONTRIBUTING.md` files inside `../suite`, `../apps/*`, `../packages/*`, or `../docs`. Keep them centralized here so GitHub inherits them across all repositories.
2. **Keep Synced with `suite/apps/www` Policy Pages:** Whenever updating ecosystem apps, SDK packages, bots, licensing, or security policies here, ensure `../suite/apps/www/src/app/{terms,privacy,cookies,security,license}/page.tsx` and `../suite/packages/lib/src/dictionaries/en-GB.json` remain 100% aligned.
