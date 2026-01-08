# Chrome DevTools MCP

## What It Is

Chrome DevTools MCP is a Model Context Protocol server that lets Claude Code directly interact with web pages in Chrome.

Claude can:
- Take snapshots of the page (accessibility tree)
- Click, type, and navigate
- Inspect network requests and console logs
- Test responsive designs
- Debug visual issues in real-time

## Why It's Powerful

Instead of just writing code and hoping it works, Claude can **see and test** the actual running application. It's like giving the AI eyes and hands.

## Installation

```bash
npx @cloudflare/mcp-server-chrome-devtools
```

Or install via the MCP settings in Claude Code:

```json
{
  "mcpServers": {
    "chrome-devtools": {
      "command": "npx",
      "args": ["-y", "@cloudflare/mcp-server-chrome-devtools"]
    }
  }
}
```

## Usage

Once installed, Claude Code can automatically use Chrome DevTools commands when you ask it to test or debug web applications.

## More Info

- [Chrome DevTools MCP on GitHub](https://github.com/cloudflare/mcp-server-chrome-devtools)
