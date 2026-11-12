@AGENTS.md

## Claude Code specifics
- The connector is in `.mcp.json`; `/mcp` lists `molclear-verifier`. A claude.ai connector
  for the elucidation agent may appear too: leave its tools alone.
- A SessionStart hook (`.claude/settings.json`) runs `scripts/setup-tools.sh`.
- `/verify <Connect-verifier text>` starts a pass.
- Claude Code on the web: the environment needs Custom network access listing
  `molclear.anthony-tong.com`, with "Also include default list of
  common package managers" ticked (PyPI, for the Python tools).
