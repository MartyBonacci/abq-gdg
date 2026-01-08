# SpecSwarm Plugin

## What It Is

SpecSwarm is a systematic workflow orchestration plugin for Claude Code that guides you through complete feature development — from specification to implementation to validation.

Instead of ad-hoc prompting, SpecSwarm provides structured workflows:
- `/specswarm-build` - Build features from spec to completion
- `/specswarm-fix` - Fix bugs with regression tests
- `/specswarm-ship` - Quality-gate validation before merging
- `/specswarm-upgrade` - Dependency upgrades with migration analysis

## Why It Matters

It's **context stacking** built into a workflow. Each step builds on the previous, ensuring the AI always has the right context at the right time.

## Installation

```bash
npx @mbonacci/specswarm-install
```

This installs SpecSwarm as an MCP server that Claude Code can use automatically.

## More Info

- [SpecSwarm on Anthropic Marketplace](https://github.com/mbonacci/specswarm)
- Created by yours truly 😎
