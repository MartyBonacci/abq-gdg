# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

This is a presentation repository for an ABQ Software Social Club / Google Developers Group talk titled "Context Stacking & The Mentor Mind" (January 8, 2026). The repository serves as both the presentation structure and workspace for live demonstrations of AI coding tools.

## Repository Purpose

This is NOT a traditional code project - it's a presentation framework where:
- Markdown files in the root define presentation sections (numbered 00-07)
- The talk demonstrates building applications from scratch using Claude Code
- Live demos show the "Magic Bullet Prompt" technique and SpecSwarm workflow
- The repository is designed to be followed along with during the presentation or used as a reference afterward

## Key Concepts Demonstrated

The presentation covers:
1. **Context Stacking** - The universal principle behind AI coding tools
2. **The Mentor Mind** - Using a second Claude Code instance to guide the first
3. **The Magic Bullet Prompt** - A meta-prompting technique (see `06-magic-bullet-prompt.md`)
4. **SpecSwarm Integration** - Building projects using the SpecSwarm plugin

## Magic Bullet Prompt Technique

The file `06-magic-bullet-prompt.md` contains a meta-prompt template for "Mentor Mind" workflows. This technique involves:
- Opening a second Claude Code instance to act as a mentor/planner
- Using that instance to generate optimized prompts for the working instance
- Leveraging SpecSwarm and other tools to build complete projects from READMEs

When working with the demo project (see `https://github.com/MartyBonacci/tweeter-gdg-1`), the Mentor Mind should:
- Read the README.md to understand project requirements
- Use AskUserQuestion tool to clarify ambiguities before starting
- Generate comprehensive prompts that utilize SpecSwarm skills and available MCP tools
- Guide the Developer instance through the full development workflow

The recommended directory structure for demonstrations:
```
tweeter-gdg-1-mentor/          # Mentor Mind opens here
  └── tweeter-gdg-1/           # Developer opens here
```

This structure ensures the Mentor Mind has a broader context than the Developer instance.

## Working with Demo Projects

The main demo project is **Tweeter** (a microblogging application):
- Repository: https://github.com/MartyBonacci/tweeter-gdg-1
- Clone and set up in a mentor/project directory structure
- Always read the README.md first to understand the project scope
- Check for project-specific CLAUDE.md files
- Use SpecSwarm skills (`/specswarm-build`, `/specswarm-ship`, etc.) for systematic development
- Leverage Chrome DevTools MCP for browser-based application testing

## Important Notes

- This repository is intentionally minimal - it's a presentation scaffold, not a complete application
- Content is added live during demonstrations
- The main value is in the conceptual framework and meta-prompting techniques, not traditional code
- When creating demos, prioritize clarity and teaching moments over production-ready code
