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

Then give the plugin your service account token. Create it in the Griffin31 dashboard, under Service accounts (it starts with `g31sa_`), and set it in Claude Code with:

```text
/plugin configure griffin31@griffin31-plugins
```

## Try it

- "Where does this tenant stand, and what should I fix first?"
- "Show me the quick wins."
- "Plan the open recommendations in the story we need to close this quarter."
- "Fix MS-ENT-31 and save the evidence."

You can also start a skill directly with `/griffin31:get-started` or `/griffin31:remediate MS-ENT-31`.

## Troubleshooting

- **Griffin31 tools fail with an authorization error:** the token is missing, wrong or revoked. Create a new one in the dashboard under Service accounts and set it again with `/plugin configure griffin31@griffin31-plugins`, then restart Claude Code.
- **No Griffin31 tools at all:** run `/mcp` and check that the `griffin31` server is connected.
- **Some recommendations show as blocked or missing:** Griffin31 can't assess what it lacks permissions or licences for. The start of every session says which; the dashboard shows how to grant them.
- **A fix doesn't show as passed:** results change only with the next scan. Check the last scan time in the dashboard.
- **Remediate stops before a change:** the browser is signed in to a different tenant than the Griffin31 account, or the portal doesn't match the steps. Sign in to the right tenant, or tell support what differs.

## Support

- [Help Center](https://kb.griffin31.com) · [Trust Center](https://kb.griffin31.com/trust-center/) · [Privacy](https://www.griffin31.com/privacy-policy/)
- Questions: [support@griffin31.ai](mailto:support@griffin31.ai)
- Security issues: see the [security policy](https://github.com/griffin31-public/.github/blob/main/SECURITY.md).

Griffin31 is a product of [OnCloud](https://www.oncld.io/en/).
