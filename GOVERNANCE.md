# Governance

## Roles

- **Contributors** anyone who sends issues, PRs, packs or docs.
- **Maintainers** review and merge changes, triage issues and cut releases. They are listed in each repository's `CODEOWNERS`.
- **Lead maintainer** breaks ties and owns the roadmap until the maintainer group has three or more members.

## Becoming a maintainer

Sustained, high-quality contributions over several months, nominated by a maintainer and approved by lazy consensus (no objection within 7 days).
Maintainers inactive for six months move to emeritus status.

## Decisions

- Small changes: PR review by one maintainer.
- Significant changes (public API, pack format, architecture, licensing, governance): an **RFC**.
- Architecture decisions are recorded as ADRs in `krama-docs/adr/`.

## RFC process

1. Open an issue with the **RFC** form: problem, proposal, alternatives, impact, migration.
2. Discussion for at least 14 days.
3. A maintainer proposes a disposition (accept, reject, postpone). Lazy consensus applies; if there is an objection, maintainers vote and a simple majority decides, with the lead breaking ties.
4. Accepted RFCs become an ADR and tracked tasks.

## Code of Conduct

Enforced per the [Code of Conduct](CODE_OF_CONDUCT.md).
