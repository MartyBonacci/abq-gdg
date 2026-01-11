# The Mentor Mind

> **Full pattern**: [github.com/MartyBonacci/four-minds-pattern](https://github.com/MartyBonacci/four-minds-pattern)

## The Pattern

Open two Claude Code instances:

1. **Mentor** - At a higher directory level (sees more)
2. **Developer** - In the project directory (does the work)

The Mentor has more context. The Developer has focus.

This is the **entry point** to the Four Minds Pattern — the simplest version that delivers immediate value.

---

## Why It Works

The **Mentor** can see:
- The entire repository structure
- Documentation in parent directories
- Setup instructions
- Multiple projects (if applicable)
- **Everything the Developer instance sees + more**

The **Developer** can see:
- Only its own directory
- What it discovers through exploration
- What you tell it directly

**The Mentor knows more. The Developer does more.**

---

## The Meta-Insight

> "Who knows Claude Code better than Claude Code?
> Another Claude Code with more context."

The Mentor uses its broader view to:
- Analyze the project requirements
- Identify available tools and workflows
- Consider what the Developer instance will need to know
- Generate the **perfect prompt** for the Developer instance

It's Claude Code writing prompts for Claude Code.

**This prevents strategic confusion during implementation** — the Developer can focus on execution while the Mentor handles strategy.

---

## When to Use This Pattern

Use the Mentor Mind when:
- Starting a new project from scratch
- You have a README or spec but no code yet
- You want to leverage tools like SpecSwarm optimally
- You're not sure what to ask for

The Mentor will ask YOU clarifying questions, then write a prompt that asks the AI clarifying questions.

**Context stacking on context stacking.**

---

## Beyond Two Instances

This pattern scales to **Four Minds**, each with a specific cognitive role:

### 1. Developer (Project Directory)
Implementation and execution. Writes code, runs tests, debugs.

### 2. Peer (Peer Directory)
Conversational brainstorming partner. Explores approaches in a safe space without commitment. Uses ideation artifacts (markdown), not code.

### 3. Mentor (Project-Mentor Directory)
Strategic advisor with dual visibility. Sees both the Developer's project AND the Peer's ideations. Crafts prompts for Developer informed by both.

### 4. Highest Self (Home Directory)
Workflow evolution partner. Sees all projects, all tools, all practices. Identifies cross-project patterns and improves your development workflow itself.

---

## The Philosophy

This isn't about decomposing tasks. It's about **separating cognitive roles**.

- **Execution** (Developer)
- **Exploration** (Peer)
- **Strategy** (Mentor)
- **Reflection** (Highest Self)

When ideation contaminates execution, use Peer. When AI outputs misalign with project patterns, use Mentor. When you're repeating mistakes across projects, use Highest Self.

**You don't need all four at once.** Start with Mentor + Developer tonight. Add the others when you need them.

**Read the full pattern**: [github.com/MartyBonacci/four-minds-pattern](https://github.com/MartyBonacci/four-minds-pattern)

---

## Try It Tonight

You don't need new tools. You just need **two terminals**.

1. Open Claude Code at the repo root (Mentor)
2. Open Claude Code in the project directory (Developer)
3. Use the Mentor to craft prompts for the Developer

That's it. That's the entry point.

When you're ready for more, add Peer and Highest Self. But start here.
