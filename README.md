# Signado for Cursor

Signado is a lead generation tool for agencies, consultants and B2B teams that sell go-to-market, digital marketing or AI services. It watches the conversations in your market on LinkedIn and tells you who to contact and what to say.

This plugin connects Cursor to your Signado workspace through Signado's hosted MCP server. Ask the agent to list warm leads with what each person said on LinkedIn, manage discovery sources, find emails, and save outreach drafts to Campaigns.

## What's included

- **MCP server:** `signado` at `https://mcp.signado.io/mcp` (streamable HTTP, OAuth sign-in)

The plugin contains no rules, skills, agents, commands, hooks or scripts.

## Install

1. Install **Signado** from the Cursor Marketplace.
2. When Cursor asks you to authenticate, sign in with your Signado account and choose the workspace to connect.

No API key is needed. To add the server without the plugin, put this in your `mcp.json`:

```json
{
  "mcpServers": {
    "signado": {
      "type": "http",
      "url": "https://mcp.signado.io/mcp"
    }
  }
}
```

## Tools

The server advertises 17 tools: `ping`, `list_warm_leads`, `get_best_of_run`, `get_warm_lead_detail`, `export_leads`, `list_hiring_leads`, `preview_source`, `add_source`, `set_source_schedule`, `run_source_once`, `cancel_source_run`, `remove_source`, `find_email`, `draft_message`, `add_hiring_lead_person`, `list_templates` and `save_template`.

Reading leads is free. Paid tools use your workspace's credits and report the credits charged in every response.

## Requirements

A Signado account. Every plan starts with a 7-day free trial.

## Links

- Product: https://signado.io/mcp?utm_source=github&utm_medium=repo&utm_campaign=cursor-plugin
- Setup guide: https://signado.io/help/mcp/mcp-overview
- Troubleshooting: https://signado.io/help/mcp/mcp-connection-issues

## License

The files in this repository are MIT licensed. The Signado service itself is proprietary.
