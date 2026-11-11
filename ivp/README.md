# IVP.ai for Claude

IVP.ai is a business data and analytics platform. This plugin connects Claude (claude.ai, Claude Desktop, Cowork and Claude Code) to your IVP.ai account, so you can ask questions about your company's data and get answers calculated on that data.

## What you can do

- Find datasets across your workspaces and see their columns
- Ask for totals, trends and rankings ("revenue by month", "top 10 customers by orders")
- Use the agreed metric definitions in your data rooms, so numbers match what your team already reports
- Preview rows with filters
- Browse dashboards and get the numbers behind any tile
- Review Deskless AI agents: latest run status, run summaries and answers searched from their outputs
- Search across agent outputs, documents and past missions, with citations back to the source
- In Claude Code, download a dataset as a CSV file to analyse in code

## What it includes

- **MCP connector** to `https://api.ivp.ai/mcp`, IVP.ai's own server. You sign in with your IVP.ai account and approve access on IVP.ai's consent page.
- **Skills:** `explore-data`, `dashboard-briefing` and `deskless-run-review`, which guide Claude through answering data questions, briefing on dashboards and reviewing agent runs.

## Access and data

- Read-only: it cannot change data, edit dashboards or run agents.
- Claude only sees the workspaces, datasets, dashboards and agents your IVP.ai account can already see.
- Data is sent from IVP.ai to Claude only in answer to your requests: query results (up to 500 aggregated rows or 50 raw rows per request), dashboard details, agent run summaries and document passages. Dataset downloads are short-lived links that expire after 15 minutes.
- Your IVP.ai plan must include the ChatGPT and Claude connection.
- You can disconnect at any time from Claude's connector settings.

## Install

In Claude Code:

```
/plugin marketplace add IVP-ai/claude-plugin
/plugin install ivp@ivp-ai
```

Then run `/mcp`, choose `ivp` and sign in.

## Links

- Documentation: https://ivp.ai
- Privacy policy: https://ivp.ai/privacy
- Terms: https://ivp.ai/terms
- Support: https://ivp.ai/contact
