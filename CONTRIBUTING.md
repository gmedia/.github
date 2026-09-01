# Contributing to GMEDIA Projects

Thanks for considering a contribution. This is the default guide for
repositories in the [GMEDIA](https://github.com/gmedia) organization.

**Individual repositories may define their own `CONTRIBUTING.md`, and theirs
takes precedence.** Repository-specific setup, test commands, and review
conventions always win over anything written here.

By participating you agree to the [Code of Conduct](CODE_OF_CONDUCT.md).

## Before you start

- Read the target project's `README` and any documentation it links to.
- Search open **and closed** issues and pull requests — your bug may be known,
  and your idea may already have been discussed.
- For anything substantial — a new dependency, a schema change, a public API
  change, a refactor across modules, a new subsystem — **open an issue first**.
  Agreeing on the approach before implementation saves everyone a rewrite.

Small, obvious fixes (a typo, a broken link, a clear one-line bug) do not need
an issue first. Just send the pull request.

## Reporting bugs

A useful bug report lets someone else reproduce the problem without asking you
follow-up questions:

- **What happened**, and **what you expected** instead.
- **Steps to reproduce**, ideally from a clean state. A minimal reproduction is
  worth more than a long description.
- **Version and environment** — commit or release, OS, runtime version,
  container versions — where relevant.
- **Logs, stack traces, or screenshots**, with secrets removed.

Redact credentials, tokens, API keys, internal hostnames, and personal or
customer data before posting. If a bug cannot be described without sensitive
data, treat it as a security report instead.

**Security vulnerabilities do not belong in issues.** Follow
[SECURITY.md](SECURITY.md).

## Pull requests

Keep the scope focused. One pull request should do one thing — a bug fix, a
feature, or a refactor, not all three. Unrelated changes bundled together are
hard to review and hard to revert.

A good pull request description explains:

- **What** changed.
- **Why** it was needed — link the issue it addresses.
- **How it was validated** — what you ran, what you observed, what you did not
  cover.

Beyond that:

- Update documentation when behaviour, configuration, or interfaces change.
- Match the existing style of the code you are touching. Leave reformatting of
  untouched code out of the diff.
- Never commit credentials, tokens, private keys, `.env` files, internal
  hostnames, or customer data. If you have already pushed one, treat it as
  compromised and rotate it.
- Expect review comments. They are about the change, not about you.

## Tests

Run the checks the repository defines — its `README`, `Makefile`, `package.json`
scripts, or CI configuration are the source of truth.

There is deliberately no single organization-wide build or test command:
projects here are written in Rust, PHP, Python, TypeScript, and Shell, and each
has its own toolchain.

Add tests for behaviour you change or add, where the project has a test suite.
If a change genuinely cannot be tested automatically, say so in the pull request
and describe how you verified it manually.

## Commit messages

Write commit messages someone can understand a year from now. A short
imperative summary line, and a body explaining *why* when the reason is not
obvious from the diff.

Where a project already uses [Conventional Commits](https://www.conventionalcommits.org/),
follow it — `feat`, `fix`, `docs`, `refactor`, `test`, `chore`. Where it does
not, clarity matters more than a prefix. Check the repository's existing history
before assuming either way.

## AI-assisted contributions

Using AI tooling to help write code is fine. We use it too.

What does not change is that **you are the author of your pull request**. By
submitting it you are taking responsibility for:

- **Correctness** — you have read the code and understand what it does.
- **Security** — you have thought about how it fails and how it could be abused.
- **Licensing** — you have the right to contribute the code under the project's
  licence.
- **Testing** — you have actually run it, not just generated it.

The practical test is simple: if a reviewer asks why a change is written the way
it is, you should be able to answer. Generated code that no one on either side
of the review understands is a maintenance liability, and we will ask you to cut
it down or explain it before merging.

Large machine-generated pull requests that were not discussed in an issue first
are likely to be closed.

## Questions

For where to ask what, see [SUPPORT.md](SUPPORT.md).
