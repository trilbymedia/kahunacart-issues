# KahunaCart Issues

The public issue tracker for [KahunaCart](https://kahunacart.com), the e-commerce plugin for Grav 2. The code lives in private repositories, so this is where bugs and feature requests go.

## Which form to use

- **Bug report** for anything broken in KahunaCart, its add-ons (Licenses, Subscriptions, Newsletters, Shipping) or the Kahuna theme.
- **Payment provider problem** for checkout, webhook, refund or subscription trouble with one specific provider. It asks for the order and provider references and the webhook state, which is what those problems turn on.
- **Feature request** for something KahunaCart does not do yet. Start with the problem you are trying to solve, not the solution.

Questions and "how do I" belong on [Discord](https://discord.gg/vMs3UTEAg4) or in the [docs](https://kahunacart.com/docs). Security reports and anything about a licence, a purchase or your account go through the [contact form](https://kahunacart.com/contact), not a public issue.

## The support report

Every bug form asks for the support report. It is a redacted dump of the store's versions, database engine, pending migrations, provider state, webhook reachability and template drift, and it answers most of the questions we would otherwise ask first. Get it either way:

- In the admin: **KahunaCart → Health → Copy support report**
- From a shell in the Grav root: `bin/plugin kahunacart check --report`

Every key, token and secret is replaced with `[redacted]` before it leaves the store, so it is safe to paste as is. Do check your log excerpts and screenshots yourself, though.

## Before you open an issue

- Search open and closed issues first.
- Update to the latest release and clear the cache with `bin/grav clearcache`. A surprising number of reports are already fixed.
- Keep one problem per issue.
