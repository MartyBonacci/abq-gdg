# Context Stacking

## The Core Principle

**The model only knows what's in its context window.**

That's it. That's the whole game.

But what's "in the window" is **more than you think**.

---

## Two Types of Context

Most people think context is just **information** — files, code, documentation.

That's only half the story.

### Information Context (What the AI Knows)

This is what everyone focuses on:
- Code files
- Documentation
- Previous messages
- Test results
- Browser snapshots

**This is passive.** It's just text in the window.

### Capability Context (What the AI Can Do)

This is what changes the game:
- **Commands** - What can be executed
- **Skills** - Workflow orchestration (like SpecSwarm)
- **Tools** - MCP servers (Chrome DevTools, file operations)
- **Subagents** - Specialized domain experts
- **Scripts and procedures** - Automated processes

**This is active.** It's action possibilities.

Both matter. Most people only stack the first.

---

## The Cascade Effect

Here's the insight that changes everything:

**When you invoke a capability, it doesn't just execute — it adds its own context.**

### Deep Dive: `/specswarm-build`

When you run this skill, watch what cascades into the context window:

**Instructions** → How to build features systematically
- "Start with a spec.md to clarify requirements"
- "Use the AskUserQuestion tool for ambiguities"
- "Generate implementation plans before writing code"

**Process Templates** → The complete workflow
- `spec.md` → Specification structure
- `plan.md` → Design artifacts
- `tasks.md` → Dependency-ordered task list
- Implementation → Execution patterns

**Validation Procedures** → Quality gates
- "Run tests before marking tasks complete"
- "Validate against the original spec"
- "Use browser testing for UI features"

**Domain Knowledge** → Best practices
- "Avoid premature optimization"
- "Write tests for business logic"
- "Use TypeScript for type safety"

**Its Own Tools** → Nested capabilities
- Analysis agents for impact assessment
- Validation workflows for quality checks
- Test runners and browser automation

You didn't just run a command.

You **imported an entire methodology** into the context.

---

### The Cascade in Action

Other examples of capabilities cascading their own context:

**Chrome DevTools MCP**
- Browser interaction protocols (how to click, fill, navigate)
- Snapshot procedures (accessibility tree formatting)
- Web accessibility knowledge (ARIA roles, semantic HTML)
- Testing processes (visual regression, interaction testing)

**Subagents (react-typescript-specialist)**
- React patterns (hooks, component composition, state management)
- TypeScript best practices (strict types, generic patterns)
- Component design knowledge (props interfaces, event handlers)
- Testing strategies (React Testing Library, user-centric tests)

**Even simple tools like Grep**
- Search strategies (regex patterns, case sensitivity)
- File filtering procedures (glob patterns, type filters)
- Output formatting knowledge (context lines, line numbers)

Every capability is a **portal to more context**.

---

## How Every AI Tool Works

Every AI coding tool—Copilot, Cursor, ChatGPT, Claude Code, Windsurf—runs on the same principle:

**Stack the right context → Get better output**

The difference isn't the LLM under the hood.

The difference is:
1. **What context** each tool can stack
2. **How easily** you can stack it

Some tools only give you information context (paste code manually).

Some tools give you both information AND capability context (skills, tools, subagents).

The more you can stack, the better the results.

---

## Why This Changes Everything

Traditional thinking:
> "I need to feed the AI more information — more code files, more documentation, more examples."

Expanded thinking:
> "I need to equip the AI with capabilities — and each capability brings its own world of context."

### See the Shift

**Bad approach** (information only):
- "Let me paste this code file so Claude knows about it"
- "Let me describe what the page looks like in detail"
- "Let me explain how our testing workflow works"

**Good approach** (capability + cascade):
- "Let me use `/specswarm-build` which brings systematic workflows"
- "Let me use Chrome DevTools MCP so Claude can see and interact with the page"
- "Let me use the test-runner subagent which knows testing best practices"

You're not just feeding information.

You're **equipping the machine with capabilities**.

And each capability cascades **its own instructions, processes, knowledge, and procedures**.

---

## The Real Question

The question isn't:
- "Which tool is best?"
- "How do I get more code in the window?"
- "Should I use Claude or GPT?"

The question is:
- **"What capabilities does this tool give me?"**
- **"What context do those capabilities cascade?"**
- **"How do I chain capabilities to stack context?"**

Once you understand this, you can make ANY AI tool more powerful.

---

## Context Stacking on Context Stacking

This is why the Mentor Mind pattern works.

It's not just that the Mentor sees more files (information context).

It's that the Mentor has **capability awareness** — it knows what tools, skills, and subagents are available, and can cascade them strategically.

The Mentor doesn't just have more information.

The Mentor knows **what's possible**.

More on that next →
