<p align="center"><img src="assets/icon.png" alt="Griffin31" width="96"></p>

# Griffin31 for Claude

See, prove and fix your Microsoft 365 security from Claude. This plugin connects Claude to your [Griffin31](https://www.griffin31.com) account: it shows where the tenant stands, picks what to fix first, and walks you through each fix in the Microsoft admin portals, saving evidence as you go.

## What you can do

- **Get started:** your score, where to begin (fix-first items, quick wins, stories and threats) and a plan for the open recommendations, with their risk, effort and the related checks to fix together.
- **Remediate:** apply one approved change at a time in the portals you're signed in to, and keep evidence of each.

Griffin31's tools only read your account. Every change in the tenant is one you approve.

## Install

```bash
claude plugin marketplace add griffin31-public/claude-plugins
```

```bash
claude plugin install griffin31@griffin31-plugins
```

Then set **Service account token** in the plugin's settings. Create the token in the Griffin31 dashboard, under Service accounts. It starts with `g31sa_`.

## Support

- [Help Center](https://kb.griffin31.com) · [Trust Center](https://kb.griffin31.com/trust-center/) · [Privacy](https://www.griffin31.com/privacy-policy/)
- Questions: [support@griffin31.ai](mailto:support@griffin31.ai)
- Security issues: see the [security policy](https://github.com/griffin31-public/.github/blob/main/SECURITY.md).

Griffin31 is a product of [OnCloud](https://www.oncld.io/en/).
