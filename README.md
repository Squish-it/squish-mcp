# Squish MCP server

Manage your [Squish](https://squish.co) account from any AI assistant: domains, DNS, hosting, backups, site files, AI Visibility and support.

This is a **hosted** server, so there is nothing to install or run. Connect your assistant to the URL below and sign in with your Squish account. This repository holds documentation only.

```
https://api.squish.co/mcp
```

- Transport: Streamable HTTP
- Auth: OAuth 2.1 (sign in with your Squish account)
- Registry: `co.squish/squish` in the [official MCP registry](https://registry.modelcontextprotocol.io)
- Full tool reference: <https://squish.co/developers>

## Connect

**Claude (claude.ai or desktop):** Settings → Connectors → Add custom connector, then paste the URL above.

**Claude Code:**

```
claude mcp add --transport http squish https://api.squish.co/mcp
```

**Cursor, VS Code and other clients:** add a remote (HTTP) MCP server with the URL above. The client opens a Squish sign-in page the first time.

## What it can do

- **Domains and DNS:** list your domains, read and edit records, set up forwarding and auto-renew, search names and prices, and prepare a registration or transfer.
- **Hosting:** see your sites and their measured uptime, the PHP version a site runs, backups and restore points, and the CDN. Read and edit the files a site serves, with a restore point taken first.
- **AI Visibility:** check how readable a site is to AI answer engines, run your report, then plan and apply fixes.
- **Support and account:** see your tickets (add a note, close, reopen), recent orders and billing address.
- **Free diagnostics for any site, no account needed:** DNS, WHOIS, SSL, uptime, security headers, blacklists, redirects, tech stack and hosting provider.

## Safety

- **Read-only by default.** Read-write access requires two-factor authentication on your Squish login.
- Every change is previewed and applied only after you confirm.
- Some actions are never available to a connection and stay in your dashboard: cancelling hosting, changing nameservers, requesting a transfer code, changing your login email and bulk DNS edits.
- Every call is logged on your account. See and revoke connections under **Dashboard → Assistant → Connected assistants**.

## Example prompts

- "Is my site's SSL certificate about to expire, and is my DNS set up right for email?"
- "Add a TXT record for Google verification on mydomain.com."
- "Take a backup, then fix the typo on my homepage."
- "How readable is my site to ChatGPT and Perplexity, and what should I fix?"
- "Check whether bakeryphx.com is available and what it costs."

## Links

- Website: <https://squish.co>
- Developer docs: <https://squish.co/developers>
- Privacy: <https://squish.co/privacy>
- Terms: <https://squish.co/terms>
- Help: <https://squish.co/help>
