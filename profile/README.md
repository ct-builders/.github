# ct-builders

**Working reference code for [commercetools](https://commercetools.com), published so you can
read it and copy from it.** Merchant Center custom applications, Connect apps, integration
patterns, and developer tooling.

Everything here is [MIT licensed](https://opensource.org/licenses/MIT), **freely available,
and unsupported**. It is written by people who work at commercetools, but it is **not a
commercetools product** — no SLA, no roadmap, no support channel. See
[Support and expectations](#support-and-expectations) before you build anything load-bearing
on it.

## What this is

Each repository is a **working application**, not a snippet or a scaffold: real
authentication, real error handling, and comments that explain *why* something is done a
particular way rather than restating what the line does. Clone one, point it at your own
commercetools project, and it runs.

The intended use is: you are building something on commercetools, you want to see how a
piece fits together before committing to a design, so you read ours first — then write your
own, or fork ours and keep going.

## What this is not

- **Not a commercetools product.** Not covered by any SLA, support contract, or roadmap
  commitment, and not part of any subscription you may have.
- **Not officially maintained.** No release schedule, no deprecation policy, no guaranteed
  response to issues or pull requests, no security patching commitment.
- **Not a replacement for anything commercetools sells.** We deliberately do not publish
  code here that overlaps a commercetools product. If there is a supported product that does
  what you need, use it — it will be better maintained than this.
- **Not something to ship unreviewed.** These implementations optimize for clarity and for
  showing a pattern end to end. Before production, you own the security review, the load
  testing, the observability, and the compliance work.
- **Not the API documentation.** For the platform itself, go to
  [docs.commercetools.com](https://docs.commercetools.com).

## Support and expectations

> This code is made freely available under the MIT License, **as is and unsupported**. There
> is no warranty, no service-level agreement, and no commitment to maintain, patch, or
> respond. commercetools Support cannot help with it. If you deploy it, you own it.

| | |
|---|---|
| **License** | MIT — use commercially, modify, redistribute; no obligation beyond keeping the notice |
| **Warranty** | None. `AS IS`, per the MIT License |
| **Support channel** | None. Not commercetools Support, not a paid tier |
| **Issues / PRs** | Read on a best-effort basis. No response-time commitment |
| **Security reports** | Please open an issue, but assume no patch timeline. Do **not** report commercetools *platform* vulnerabilities here — use [commercetools' security contact](https://commercetools.com/privacy-and-security) |
| **Breaking changes** | Possible at any time, without notice or a migration path |
| **Maintenance** | Not guaranteed to continue. A repository may be archived without warning |
| **Production use** | Entirely at your own risk, after your own review |

Every source file in every repository carries an SPDX header saying the same thing, so the
terms travel with the code even when one file gets copied out of context:

```
/*
 * SPDX-License-Identifier: MIT
 * Copyright (c) 2026 commercetools GmbH and the ct-builders contributors
 * Freely available, AS IS and UNSUPPORTED. See LICENSE.
 */
```

## Using a repository

Each repo has its own README, but the shape is consistent:

1. Create or pick a commercetools project.
2. Create an API client scoped to what that app actually needs — never a `manage_project`
   client for a deployed app.
3. Copy `.env.example` to `.env` and fill it in.
4. Install and run.

**No repository here contains credentials, and none ever should.** If you find a secret in
this org's git history, please open an issue immediately.

## Contributing

Contributions are welcome, with two hard requirements:

1. **Every source file carries the SPDX header above** — including files you only edited. The
   header is what makes the terms survive a copy-paste.
2. **You may only contribute code you have the right to license under MIT.** Do not paste in
   code from another project, a customer engagement, or a vendor's repository unless its
   license permits it and you preserve the original notice.

Beyond that: no customer names, no credentials, no internal infrastructure references, no
personal data — these repositories are public, permanently, git history included.

See `CONTRIBUTING.md` in any repository for the full checklist.

## Relationship to commercetools

The code here is written by commercetools employees, and the copyright is held by
commercetools GmbH and the contributors to this org. That is the extent of the relationship.
Publication here is **not** an endorsement, a support commitment, or a statement that this is
how commercetools recommends you build. Treat it as well-informed reference code from
practitioners, and make your own architectural decisions.

---

**Looking for the officially supported thing instead?**
[Documentation](https://docs.commercetools.com) ·
[commercetools on GitHub](https://github.com/commercetools) ·
[Support portal](https://support.commercetools.com)
