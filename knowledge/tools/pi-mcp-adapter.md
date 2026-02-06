# pi-mcp-adapter

**URL:** https://github.com/nicobailon/pi-mcp-adapter

**Author:** nicobailon

**Stars:** 46

**Language:** TypeScript

**Topics:** ai, claude, coding-agent, extension, llm, mcp, model-context-protocol, pi

## Summary

Token-efficient MCP adapter for Pi coding agent. Solves the problem of MCP tool definitions burning excessive context tokens (10k+ per server) by providing a lightweight proxy tool (~200 tokens) that discovers tools on-demand. Servers only start when their tools are actually used.

## Key Features

- **Lazy loading by default** — MCP servers don't connect until you actually call their tools
- **Metadata caching** — search and describe work without live connections
- **Configurable lifecycle modes** — lazy, eager, or keep-alive
- **Direct tool promotion** — optional TUI panel to elevate specific MCP tools to first-class status
- **Idle timeout management** — automatic disconnection after configurable inactivity periods
- **Resource exposure** — MCP resources can be exposed as tools

## Installation

```bash
pi install npm:pi-mcp-adapter
```

## Configuration

Create `~/.pi/agent/mcp.json` to define MCP servers. Key options:

- **lifecycle** — "lazy" (default), "eager", or "keep-alive"
- **idleTimeout** — Minutes before idle disconnect
- **directTools** — Register tools individually (true, false, or array of tool names)
- **toolPrefix** — "server", "short", or "none"

## Use Cases

- Running multiple MCP servers without token bloat
- Selective promotion of frequently-used MCP tools to first-class status
- Dynamic tool discovery and exploration without pre-loading definitions
- Serverless tool integration with the Pi coding agent

## Related

- **pi-subagents** — Can be configured to load specific MCP tools for subagents
