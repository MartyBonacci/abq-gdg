# Context Stacking & The Mentor Mind

Learn how to use Claude Code more effectively by understanding context stacking and the Mentor Mind pattern.

---

## Watch the Video

> **YouTube video coming soon**
>
> This repository serves as the reference material for the video. Watch first, then use this repo to dig deeper.

---

## What You'll Learn

- **Context Stacking** — Why some prompts work better than others
- **The Mentor Mind** — Using two Claude Code instances for better results
- **The Magic Bullet Prompt** — The template I use on every project

---

## Quick Start

Want to try the Mentor Mind pattern right now?

1. **Setup** (if you haven't already):
   - [Claude Code Setup](00-setup/claude-code.md)
   - [SpecSwarm Plugin](00-setup/specswarm.md)
   - [Chrome DevTools MCP](00-setup/chrome-devtools.md)

2. **Clone the demo project:**
   ```bash
   mkdir tweeter-gdg-1-mentor
   cd tweeter-gdg-1-mentor
   git clone https://github.com/MartyBonacci/tweeter-gdg-1.git
   ```

3. **Open two Claude Code instances:**
   - Mentor: `tweeter-gdg-1-mentor/`
   - Developer: `tweeter-gdg-1-mentor/tweeter-gdg-1/`

4. **Use the Magic Bullet Prompt** (in the Mentor instance):
   ```
   Please ultrathink and help me write a prompt to give to a Claude Code
   instance opened in tweeter-gdg-1-mentor/tweeter-gdg-1 to best use
   SpecSwarm and all other available commands, skills, tools, and
   resources to build the project described in the README.md file.

   Please use the AskUserQuestion tool to ask any clarifying questions
   to fill in any missing information that you are not 96% confident
   about to complete the project.
   ```

---

## Reference Material

| # | Topic | Description |
|---|-------|-------------|
| 1 | [The Demo](reference/02-the-demo.md) | Step-by-step demo instructions |
| 2 | [The Expressibility Gap](reference/03-expressibility-gap.md) | Why we can't say what we mean |
| 3 | [Context Stacking](reference/04-context-stacking.md) | Information + Capability + Cascade |
| 4 | [The Mentor Mind](reference/05-mentor-mind.md) | The four minds pattern |
| 5 | [Magic Bullet Prompt](reference/06-magic-bullet-prompt.md) | The template that works every time |
| 6 | [Resources](reference/07-resources.md) | Links and further reading |

---

## Related Repositories

- [tweeter-gdg-1](https://github.com/MartyBonacci/tweeter-gdg-1) — Demo starter project
- [expressibility-gap](https://github.com/MartyBonacci/expressibility-gap) — Deep dive on the expressibility gap
- [four-minds-pattern](https://github.com/MartyBonacci/four-minds-pattern) — The complete four minds framework

---

## About

**Marty Bonacci**
Lead Instructor, Deep Dive Coding • Creator of SpecSwarm

- [LinkedIn](https://linkedin.com/in/martybonacci)
- [GitHub](https://github.com/MartyBonacci)

---

## Origin

Originally presented at ABQ Software Social Club / Google Developers Group on January 8, 2026.
