# Recording Outline

Step-by-step flow for recording the YouTube video. Follow these instructions naturally—explain what you're doing as you do it.

---

## Opening (~2 min)

1. Introduce yourself
   - Lead Instructor at Deep Dive Coding
   - Creator of SpecSwarm
2. What viewers will learn
   - How to use Claude Code more effectively
   - The "Mentor Mind" pattern for building projects from scratch
   - Context stacking: why some prompts work better than others
3. Mention the reference repo (link in description)

---

## Section 1: The Demo (~10 min)

**Goal:** Build a microblogging app from just a README

### Setup
1. Create the Mentor Mind directory structure:
   ```bash
   mkdir tweeter-gdg-1-mentor
   cd tweeter-gdg-1-mentor
   git clone https://github.com/MartyBonacci/tweeter-gdg-1.git
   ```
2. Show the structure: mentor directory contains the project

### The Two Instances
3. Open Claude Code in `tweeter-gdg-1-mentor/` (this is the Mentor)
4. Open Claude Code in `tweeter-gdg-1-mentor/tweeter-gdg-1/` (this is the Developer)
5. Explain: Mentor sees more context (the outer directory)

### The Magic Bullet Prompt
6. In the Mentor instance, paste:
   ```
   Please ultrathink and help me write a prompt to give to a Claude Code
   instance opened in /path/to/tweeter-gdg-1 to best use SpecSwarm and
   all other available commands, skills, tools, and resources to build
   the project described in the README.md file.

   Please use the AskUserQuestion tool to ask any clarifying questions
   to fill in any missing information that you are not 96% confident
   about to complete the project.
   ```
7. Answer its clarifying questions
8. Copy the generated prompt to the Developer instance
9. Watch it build

---

## Section 2: Why It Works (~5 min)

**Key Point:** The Expressibility Gap

1. We can't say what we mean perfectly
   - Gap between what we envision and what we can articulate
   - Not a character limit—a cognitive limit
2. The Mentor Mind bridges this gap
   - Asks the right questions (AskUserQuestion tool)
   - Knows what Claude Code can do
   - Writes better prompts than we can

Reference: [expressibility-gap repo](https://github.com/MartyBonacci/expressibility-gap)

---

## Section 3: Context Stacking (~8 min)

**Key Point:** The model only knows what's in its context window

### Two Types of Context

1. **Information Context** (passive)
   - Code files, documentation, previous messages
   - Just text in the window

2. **Capability Context** (active)
   - Commands, skills, tools, subagents
   - Action possibilities

### The Cascade Effect

3. When you invoke a capability, it adds its own context
   - Example: `/specswarm:build`
     - Loads the build skill instructions
     - Accesses spec.md template
     - Can spawn exploration agents
     - Uses SpecSwarm-specific patterns

4. This is why some prompts work better
   - They trigger capabilities that bring more context
   - Context stacking = layered enhancement

---

## Section 4: The Mentor Mind (~5 min)

**Key Point:** Two instances, different contexts

### The Four Minds Pattern
1. Developer - Does the work (narrow focus)
2. Peer - Reviews and collaborates
3. Mentor - Guides with broader context
4. Highest Self - Strategic planning

### For This Demo
5. Focus on Developer + Mentor
   - Mentor at repo root (sees everything)
   - Developer in project directory (focused execution)
6. Directory structure creates the context difference

Reference: [four-minds-pattern repo](https://github.com/MartyBonacci/four-minds-pattern)

---

## Section 5: The Magic Bullet Prompt (~5 min)

**Key Point:** One prompt template for any project

### The Template
1. Show the template again
2. Break down why each part matters:
   - "ultrathink" → triggers plan mode
   - "best use SpecSwarm and all other available tools" → capability awareness
   - "AskUserQuestion tool" → fills the expressibility gap
   - "96% confident" → the sweet spot threshold

### Variations
3. Show the bug-fixing version (`/specswarm:fix`)
4. Show the upgrade version (`/specswarm:upgrade`)
5. Same pattern, different workflows

---

## Closing (~2 min)

### Three Key Takeaways
1. **Context is everything** - What's in the window matters
2. **Capabilities cascade** - Tools bring their own context
3. **The Mentor Mind works** - Two instances > one instance

### Resources
1. This repo (link in description)
2. SpecSwarm plugin: `/plugin install specswarm@MartyBonacci`
3. Chrome DevTools MCP: `/plugin install chrome-devtools-mcp`
4. Four Minds Pattern repo
5. Expressibility Gap repo

### Call to Action
- Try the Mentor Mind pattern tonight
- Start with a simple project README
- See what Claude Code builds

---

## Recording Notes

- Keep it conversational, not scripted
- Pause after each major concept
- Show don't tell—the demo should speak for itself
- If something breaks during the demo, explain how to debug it
- Timestamps can be added in post for YouTube chapters
