# SpecSwarm

## What It Is

SpecSwarm is a complete software development toolkit for Claude Code. Created by Marty Bonacci, it guides you through the entire development lifecycle — from specification to implementation to validation.

Instead of ad-hoc prompting, SpecSwarm provides structured workflows that build on each other, ensuring Claude always has the right context at the right time.

**Supports 6 languages**: JavaScript/TypeScript, Python, PHP, Go, Ruby, Rust

## Core Workflows

The 5 essential commands:

- **`/specswarm:init`** — Initialize project with configuration files
- **`/specswarm:build`** — Build features from spec to completion
- **`/specswarm:fix`** — Fix bugs with regression testing
- **`/specswarm:modify`** — Change existing features with impact analysis
- **`/specswarm:ship`** — Quality validation and merge to main

Plus 27+ advanced commands for specialized workflows.

## Why It Matters

**Context stacking built into a workflow.**

Each SpecSwarm command cascades its own:
- Instructions (how to approach the task systematically)
- Process templates (spec.md → plan.md → tasks.md → implementation)
- Validation procedures (quality gates, test requirements)
- Domain knowledge (best practices, patterns, anti-patterns)

You're not just running a command — you're **importing an entire methodology** into Claude's context.

## Key Features

- **Quality Validation** — Automated 0-100 point scoring across tests, coverage, bundle size, and visual alignment
- **Tech Stack Drift Prevention** — 95% drift prevention through automatic pattern validation
- **Natural Language Interface** — Describe tasks conversationally or use commands
- **SSR Pattern Validation** — Detects production failures before deployment
- **Chain Bug Detection** — Prevents cascading test failures
- **Bundle Size Monitoring** — Automatic performance tracking

## Installation

In Claude Code, run:

```
/plugin install specswarm@MartyBonacci
```

That's it! Claude Code will handle the rest.

## Usage

Once installed, you can use SpecSwarm workflows directly:

```
/specswarm:build
```

Or just describe what you want in natural language:
- "Build a user authentication feature"
- "Fix the bug where the form doesn't submit"
- "Add dark mode to the settings page"

SpecSwarm will guide Claude through the complete workflow.

## More Info

- **Repository**: [SpecSwarm on GitHub](https://github.com/MartyBonacci/specswarm)
- **Current Version**: v3.7.1 (2026-01-08)
- **Author**: Marty Bonacci (that's me!)
