# Contributing to Krama

Thanks for helping. This guide applies to every repository in the `kramahq` organization.

## Picking a task

- Look for issues labelled `good first issue` or `help wanted`.
- Comment on the issue to claim it before starting. If there is no activity for two weeks, it is free again.
- For anything larger than a small fix, open an issue (or an RFC, see [GOVERNANCE.md](GOVERNANCE.md)) before writing code.

## Development flow

1. Fork the repository and create a branch from `main` (`feat/short-name`, `fix/short-name`).
2. Make your change with tests. Keep the PR focused on one thing.
3. Run the repository's checks (`pnpm install && pnpm build && pnpm test && pnpm lint` for `krama`).
4. Open a pull request using the template. CI must be green on Linux, macOS and Windows.
5. A maintainer reviews. Address comments with new commits; we squash on merge.

## Commit messages: Conventional Commits

Use the form `type(scope): summary`, for example `feat(engine): cap revise loops`.
Types: `feat`, `fix`, `docs`, `refactor`, `test`, `build`, `ci`, `chore`.
Mark breaking changes with `!` and a `BREAKING CHANGE:` footer.

## Developer Certificate of Origin (DCO)

We do not use a CLA. Every commit must carry a sign-off certifying the [DCO](https://developercertificate.org/):

```
git commit -s -m "fix(sdk): retry on 503"
```

This adds `Signed-off-by: Your Name <you@example.com>`. A check blocks PRs with unsigned commits. To fix, run `git rebase --signoff main` and force-push your branch.

## Standards

- Code works on Windows, Linux and macOS. No bash scripts, native modules or hand-built paths.
- Add or update tests and docs with behaviour changes. Add a changeset for published packages.
- Never commit secrets.

## Licence

Contributions are licensed under Apache-2.0, the licence of the repository you contribute to.

## Conduct and security

Be kind: see the [Code of Conduct](CODE_OF_CONDUCT.md). Report vulnerabilities privately: see [SECURITY.md](SECURITY.md).
