# ct-builders

Reference implementations for [commercetools](https://commercetools.com) — storefronts,
Merchant Center custom applications, Connect apps, and the integration patterns that sit
between them.

This code was written to be read. Each repository is a working application, not a snippet
or a scaffold: real authentication, real cart and checkout flows, real error handling, and
comments that explain why something is done a particular way rather than restating what the
line does. If you are building on commercetools and want to see how a piece fits together
before you commit to a design, start here.

## What this org is

**Working reference code, published so you can copy from it.** Clone a repo, point it at
your own commercetools project, and it runs. Read it, fork it, lift the parts you need.

Everything here is released under the [MIT License](https://opensource.org/licenses/MIT)
and is **unsupported**. See [Support and expectations](#support-and-expectations) below —
please read it before you build something load-bearing on top of this.

## What this org is not

- **Not a commercetools product.** Nothing here is covered by a commercetools SLA, support
  contract, or roadmap commitment. It is not part of any subscription you may have.
- **Not officially maintained.** There is no release schedule, no deprecation policy, no
  guaranteed response to issues or pull requests, and no security patching commitment.
- **Not a starting point you should ship unreviewed.** These implementations optimize for
  clarity and for demonstrating a pattern end to end. Before production you own the
  security review, the load testing, the observability, and the compliance work.
- **Not the API documentation.** For the platform itself, go to
  [docs.commercetools.com](https://docs.commercetools.com).

## Support and expectations

> This code is made freely available under the MIT License, **as is and unsupported**.
> There is no warranty, no service-level agreement, and no commitment to maintain, patch,
> or respond. commercetools support cannot help with it. If you deploy it, you own it.

Concretely:

| | |
|---|---|
| **License** | MIT — use it commercially, modify it, redistribute it, no attribution beyond the license notice |
| **Warranty** | None. `AS IS`, per the MIT License |
| **Support channel** | None. Not commercetools Support, not a paid tier |
| **Issues / PRs** | Read on a best-effort basis. No response-time commitment |
| **Security reports** | Please still open an issue, but assume no patch timeline. Do not report platform vulnerabilities here — use commercetools' official channel |
| **Breaking changes** | Possible at any time, without notice or a migration path |
| **Production use** | Entirely at your own risk, after your own review |

Every source file in every repository carries an SPDX header saying the same thing, so the
terms travel with the code even when a single file gets copied out of context.

## Using a repository

Each repo has its own README with setup steps, but the shape is consistent:

1. Create or pick a commercetools project.
2. Create an API client scoped to what that app actually needs — never a `manage_project`
   client for a deployed app.
3. Copy `.env.example` to `.env` and fill it in.
4. Install and run.

None of these repositories contain credentials, and none should ever have them committed.
If you find a secret in this org's git history, please open an issue immediately.

## Contributing

Contributions are welcome, with two hard requirements:

1. **Every source file carries the SPDX license header.** No exceptions, including files
   you only touched. The header is what makes the terms survive a copy-paste.
2. **You may only contribute code you have the right to license under MIT.** Do not paste
   in code from another project, a customer engagement, or a vendor's repository unless its
   license permits it and you preserve the original notice.

Beyond that: no customer names, no credentials, no internal infrastructure references, and
no customer-confidential data — public repo, public forever, git history included.

See `CONTRIBUTING.md` in any repository for the full checklist.

## Relationship to commercetools

These repositories are written by people who work at commercetools, and the copyright is
held by commercetools GmbH and the contributors to this org. That is the extent of the
relationship. Publication here is **not** an endorsement, a support commitment, or a
statement that this is how commercetools recommends you build. Treat it as well-informed
reference code from practitioners, and make your own architectural decisions.

---

**Looking for the officially supported thing instead?**
[commercetools documentation](https://docs.commercetools.com) ·
[commercetools GitHub](https://github.com/commercetools) ·
[Support portal](https://support.commercetools.com)
