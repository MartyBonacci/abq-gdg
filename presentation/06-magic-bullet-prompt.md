# The Magic Bullet Prompt

This is the prompt I use on **every project** when starting from scratch.

---

## The Template

Paste this into the **Mentor Mind** instance (opened at the repository root):

```
Please ultrathink and help me write a prompt to give to a Claude Code instance
opened in [PROJECT_DIRECTORY] to best use SpecSwarm and all other available
commands, skills, tools, and resources to build the project described in the
README.md file.

Please use the AskUserQuestion tool to ask any clarifying questions to fill in
any missing information that you are not 96% confident about to complete the
project — things I have missed, have not considered, or don't know will need
more information.
```

Replace `[PROJECT_DIRECTORY]` with the actual path, like:
- `/home/marty/code-projects/tweeter-gdg-1-mentor/tweeter-gdg-1`

---

## What It Does

The Mentor Mind will:

1. **Enter plan mode** (because you said "ultrathink")
2. **Read the README.md** in the project directory
3. **Analyze available tools**:
   - SpecSwarm skills (`/specswarm-build`, `/specswarm-fix`, etc.)
   - MCP servers (Chrome DevTools, filesystem, etc.)
   - Subagents (Explore, Plan, React TypeScript Specialist, etc.)
4. **Ask YOU clarifying questions** using the AskUserQuestion tool
   - What's the target audience?
   - Should it support auth? What kind?
   - What's the deployment target?
   - Any specific libraries or patterns to use/avoid?
5. **Generate a comprehensive prompt** for the Project instance

---

## Why Each Part Matters

### "Ultrathink"

This triggers **plan mode** in Claude Code. The Mentor will:
- Thoroughly explore the codebase
- Read all relevant files
- Think through the approach before responding
- Give you a well-reasoned plan

### "Best use SpecSwarm and all other available tools"

This tells Claude to:
- Leverage systematic workflows (SpecSwarm)
- Use subagents for specialized tasks
- Take advantage of MCP servers
- Not just write code manually — **orchestrate**

### "AskUserQuestion tool"

This is the key to **filling the expressibility gap**.

Instead of guessing what you want, Claude will:
- Identify ambiguities in the README
- Ask specific questions about missing requirements
- Get a 96% confidence level before proceeding

You answer the questions. It writes the perfect prompt.

### "Not 96% confident"

This threshold is intentional:
- Not 100% (impossible — it would ask forever)
- Not 50% (too many guesses)
- 96% is the sweet spot — clarify the important stuff, infer the obvious

---

## The Output

The Mentor Mind will generate something like:

```
I will now build the Tweeter microblogging application. Here's my approach:

1. Use /specswarm-build to create a complete feature specification
2. Implement the tech stack: React Router v7, PostgreSQL, Node.js
3. Use the react-typescript-specialist subagent for component development
4. Test with Chrome DevTools MCP for visual validation
5. Ship with /specswarm-ship for quality gates

[Detailed breakdown of architecture, data models, features, etc.]

Please confirm this approach, and I'll proceed.
```

You paste **that** into the Project Instance, and it starts building.

---

## Why This Works

The Mentor Mind has:
- **Broader context** (sees the whole repo)
- **Knowledge of Claude Code's capabilities** (because it IS Claude Code)
- **Your clarifications** (from the questions it asked)

It writes a prompt that the Project Instance can execute **perfectly**.

**Context stacking at its finest.**

---

## Variations

You can adapt this for different scenarios:

### Bug Fixing
```
Please ultrathink and help me write a prompt to give to a Claude Code instance
to debug and fix [ISSUE_DESCRIPTION] using /specswarm-fix and available tools.
```

### Upgrades
```
Please ultrathink and help me write a prompt to upgrade [DEPENDENCY] in
[PROJECT_DIRECTORY] using /specswarm-upgrade.
```

### Refactoring
```
Please ultrathink and help me write a prompt to refactor [MODULE] in
[PROJECT_DIRECTORY] using /specswarm-refactor.
```

Same pattern. Different workflow.

---

## Try It Right Now

1. Clone the starter repo: `git clone https://github.com/MartyBonacci/tweeter-gdg-1.git`
2. Create a mentor directory structure (see `02-the-demo.md` for details)
3. Start Claude Code in the mentor directory (Mentor Mind)
4. Paste the template (point it at `tweeter-gdg-1-mentor/tweeter-gdg-1`)
5. Answer its questions
6. Copy the output
7. Open Claude Code in `tweeter-gdg-1-mentor/tweeter-gdg-1/` (Developer)
8. Paste and watch it build

That's the magic bullet.



I used this on 1/8/26


Please ultrathink and help me write a prompt to give to a Claude Code instance opened in             
  /home/marty/code-projects/tweeter-gdg-1-mentor/tweeter-gdg-1 to best use specswarm and all other     
  avilable commands, skills, tools and resources to build the project described in the README.md file. 
  Please us the askuserquestions tool to ask any clarifying questions to fill in any missing           
  information that you are not 96% confident about to complete the project, that I have missed, have   
  not considered or don't know will need more information.