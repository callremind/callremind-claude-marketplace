# CallRemind — Claude Code Plugin Marketplace

Self-hosted [Claude Code plugin marketplace](https://code.claude.com/docs/en/plugin-marketplaces) for CallRemind.
It adds the **CallRemind MCP server** + a usage skill so Claude Code can place AI voice calls,
schedule reminders, and manage agents/leads/notifications on your CallRemind account.

## Publish (one-time)

```bash
# 1) Init + push this folder to a public GitHub repo
git init
git add .
git commit -m "CallRemind Claude Code plugin marketplace"
git remote add origin git@github.com:callremind/claude-plugin-marketplace.git
git push -u origin main
```

## Install (for end users)

```bash
/plugin marketplace add callremind/claude-plugin-marketplace
/plugin install callremind@callremind
```

Or open **Claude Code → Plugins → Marketplaces → Add** and paste the GitHub repo.
Then in a project, start with **Claude Code**, choose the CallRemind scope, and sign in
(email OTP / GitHub / Google).

## Structure

```
.claude-plugin/marketplace.json            # marketplace catalog
plugins/callremind/
  .claude-plugin/plugin.json               # plugin manifest
  .mcp.json                                # adds CallRemind remote MCP server
  skills/callremind/SKILL.md               # usage guide skill
```

## Updates
- Bump `version` in `marketplace.json` + `plugin.json` on each release; users run `/plugin marketplace update`.