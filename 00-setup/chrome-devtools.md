# Chrome DevTools MCP

## What It Is

Chrome DevTools MCP is the official Google Chrome DevTools plugin for Claude Code. It's a Model Context Protocol (MCP) server that lets Claude directly interact with web pages in Chrome.

Claude can:
- Take snapshots of the page (accessibility tree)
- Click, type, and navigate
- Inspect network requests and console logs
- Analyze performance with Chrome DevTools profiling
- Test responsive designs
- Debug visual issues in real-time

## Why It's Powerful

Instead of just writing code and hoping it works, Claude can **see and test** the actual running application. It's like giving the AI eyes and hands.

Built on Puppeteer for reliable automation, the plugin provides the same debugging power you use manually — but automated through Claude Code.

## Installation

In Claude Code, run:

```
/plugin install chrome-devtools-mcp
```

That's it! Claude Code will handle the rest.

## Usage

Once installed, Claude Code can automatically use Chrome DevTools commands when you ask it to test or debug web applications.

Just ask Claude to:
- "Test the login form in the browser"
- "Take a screenshot of the homepage"
- "Check the network requests when I click submit"
- "Debug why the button isn't appearing"

Claude will launch Chrome, interact with your app, and report back what it finds.

## More Info

- **Repository**: [Chrome DevTools MCP on GitHub](https://github.com/ChromeDevTools/chrome-devtools-mcp)
- **Author**: Google LLC (Chrome DevTools Team)
- **Current Version**: 0.12.1
