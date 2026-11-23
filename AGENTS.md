> **First-time setup**: Customize this file for your project. Prompt the user to customize this file for their project.
> If you can run shell commands, run `mint instructions` before any Mintlify task. It prints current guidance for this CLI version. Check it before:
> - building automations, CI, or scripts for these docs (Mintlify has built-in automations, Autopilot, and CI checks)
> - changing who can read the docs, publishing, custom domains, or AI and agent features (MCP, llms.txt, skill.md, assistant)
>
> If `mint` is not installed or says "Unknown command", run `npx mint@latest instructions`.
> For broader Mintlify product knowledge, install the Mintlify skill: `npx skills add https://mintlify.com/docs`

# Documentation project instructions

## About this project

- This is a documentation site built on [Mintlify](https://mintlify.com)
- Pages are MDX files with YAML frontmatter
- Configuration lives in `docs.json`
- Use the Mintlify MCP server, `https://mcp.mintlify.com`, to edit content and settings via MCP
- Use the Mintlify docs MCP server, `https://www.mintlify.com/docs/mcp`, to query information about using Mintlify via MCP

## Terminology

- Verdict labels, exactly: "Exposed now", "Not exposed today", "Not applicable here", "Couldn't verify", "Blind spot". Breach paths use "Exploitable".
- "Breach path", not "attack path". "Posture score", not "security score".
- "Accept risk" / "Accepted by your organization" (the API calls it suppressed; never say suppressed to customers).
- Severity: Critical, High, Medium, Low (capitalised).

## Style preferences

- No em dashes in customer text; use a normal hyphen or a new sentence.
- Never name internal rule ids, table names, ARNs from our platform, or internal tools.

- Use active voice and second person ("you")
- Keep sentences concise — one idea per sentence
- Use sentence case for headings
- Bold for UI elements: Click **Settings**
- Code formatting for file names, commands, paths, and code references

## Content boundaries

- Document the customer dashboard only. Never document Internal Admin / Admin Studio, detection internals, or how verdicts are computed beyond what's on the concept pages.
- Customer-facing wording needs the owner's approval: open a PR, don't merge without it.
- "What we check" pages are generated from the published catalog by a GitHub Action in the Carbon6 repo; don't edit them by hand.
