# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

This is a reference repository for teaching "Context Stacking & The Mentor Mind" — originally presented at ABQ Software Social Club / Google Developers Group (January 8, 2026), now adapted for YouTube.

## Repository Structure

```
abq-gdg/
├── README.md              # Hub for viewers
├── CLAUDE.md              # This file
├── RECORDING-OUTLINE.md   # Step-by-step outline for recording
├── 00-setup/              # Setup guides
│   ├── claude-code.md
│   ├── specswarm.md
│   └── chrome-devtools.md
└── reference/             # Detailed reference material
    ├── 00-intro.md
    ├── 01-audience-check-in.md
    ├── 02-the-demo.md
    ├── 03-expressibility-gap.md
    ├── 04-context-stacking.md
    ├── 05-mentor-mind.md
    ├── 06-magic-bullet-prompt.md
    └── 07-resources.md
```

## Key Concepts

1. **Context Stacking** - Information context (passive) + Capability context (active) + Cascade effect
2. **The Mentor Mind** - Two Claude Code instances with different context visibility
3. **The Magic Bullet Prompt** - Meta-prompting technique (see `reference/06-magic-bullet-prompt.md`)
4. **SpecSwarm Integration** - Building projects using the SpecSwarm plugin

## Magic Bullet Prompt Technique

The file `reference/06-magic-bullet-prompt.md` contains the meta-prompt template for "Mentor Mind" workflows:

```
Please ultrathink and help me write a prompt to give to a Claude Code instance
opened in [PROJECT_DIRECTORY] to best use SpecSwarm and all other available
commands, skills, tools, and resources to build the project described in the
README.md file.

Please use the AskUserQuestion tool to ask any clarifying questions to fill in
any missing information that you are not 96% confident about to complete the
project.
```

The recommended directory structure for demonstrations:
```
tweeter-gdg-1-mentor/          # Mentor Mind opens here
  └── tweeter-gdg-1/           # Developer opens here
```

## Demo Project

The main demo project is **Tweeter** (a microblogging application):
- Repository: https://github.com/MartyBonacci/tweeter-gdg-1
- Clone into a mentor directory structure
- Use SpecSwarm skills (`/specswarm:build`, `/specswarm:ship`, etc.)
- Leverage Chrome DevTools MCP for browser testing

## Related Repositories

- [tweeter-gdg-1](https://github.com/MartyBonacci/tweeter-gdg-1) - Demo starter project
- [expressibility-gap](https://github.com/MartyBonacci/expressibility-gap) - The expressibility gap concept
- [four-minds-pattern](https://github.com/MartyBonacci/four-minds-pattern) - The complete four minds framework
