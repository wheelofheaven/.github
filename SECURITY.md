# Security Policy

This policy covers every repository in the [`wheelofheaven`](https://github.com/wheelofheaven)
organisation, and is the contact channel named in
[`security.txt`](https://www.wheelofheaven.world/.well-known/security.txt).

## Reporting a vulnerability

**Use GitHub's private vulnerability reporting** — open the **Security**
tab on the affected repository and choose **Report a vulnerability**. That
keeps the report private until a fix is out, and no email address has to
be published for scrapers to harvest.

If you cannot use that form, write via the
[contact page](https://www.wheelofheaven.world/contact/) and say only that
you have a security report — please don't put the details in a public
channel.

Please include what you need to make the issue reproducible: the affected
URL or package version, what you did, and what happened. A proof of
concept helps enormously. You do not need to have a fix.

## What we can commit to

This is a small, volunteer-run project, so an honest expectation rather
than a corporate SLA:

- **Acknowledgement:** within 7 days.
- **Assessment:** within 30 days, including whether we consider it in
  scope and what we intend to do.
- **Disclosure:** we will credit you when the fix ships, unless you would
  rather stay anonymous. There is no bug bounty.

## Scope

The interesting surfaces, roughly in order of how much a report would
matter to us:

| Surface | Why it's worth reporting |
|---|---|
| [`@wheelofheaven/mcp`](https://www.npmjs.com/package/@wheelofheaven/mcp) | Published npm package — runs on other people's machines. Supply-chain issues here have real reach. |
| `mcp.wheelofheaven.world` | Cloudflare Worker. Read-only and unauthenticated, but it is code we run. |
| Client-side JS on `www` / `docs` | XSS, and anything that lets one visitor affect another. We have shipped an XSS before and want to hear about the next one. |
| DNS and domain configuration | Subdomain takeover on any `*.wheelofheaven.world` host. |

**Out of scope**, and please don't spend your time on them:

- Missing hardening headers with no demonstrated impact, and
  "best-practice" scanner output generally. We know; we are working
  through it deliberately.
- Anything that requires a compromised device or a browser extension.
- Denial of service and volumetric testing. Please do not.
- Absence of authentication. There is none by design — the corpus is
  public domain, and this is stated at
  [`/.well-known/auth.md`](https://www.wheelofheaven.world/.well-known/auth.md).
- Social engineering of contributors.

## Content is not a security issue

The corpus argues for an unconventional reading of ancient texts. That is
an editorial matter, not a vulnerability. Corrections and criticism are
genuinely welcome — as
[issues](https://github.com/wheelofheaven/www.wheelofheaven.world/issues),
not security reports.

## Licence

Everything here is [CC0-1.0](https://creativecommons.org/publicdomain/zero/1.0/).
Reporting a vulnerability does not sign anything away and does not require
you to agree to anything.
