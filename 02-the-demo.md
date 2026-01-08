# The Live Demo

Watch me build a microblogging app (Tweeter) from scratch using just a README and two Claude Code instances.

## Setup

### Step 1: Clone the Starter Repo

```bash
git clone https://github.com/MartyBonacci/tweeter-gdg-1.git
cd tweeter-gdg-1
```

### Step 2: Create a Mentor Directory

The Mentor Mind needs to see MORE than just the project:

```bash
cd ..
mkdir tweeter-gdg-1-mentor
cd tweeter-gdg-1-mentor
```

Now symlink or copy the project into this directory:

```bash
ln -s ../tweeter-gdg-1 tweeter-gdg-1
# OR
cp -r ../tweeter-gdg-1 .
```

Your structure should look like:
```
tweeter-gdg-1-mentor/
  └── tweeter-gdg-1/     # The actual project
```

### Step 3: Open the Mentor Mind

Open Claude Code at the **mentor directory**:

```bash
cd /path/to/tweeter-gdg-1-mentor
claude
```

This instance can see:
- The entire mentor directory structure
- The tweeter-gdg-1/ project subdirectory
- Any documentation you add at the mentor level
- **Everything the project will see + the parent context**

### Step 4: Open the Developer Instance

In a new terminal, open Claude Code in the **project directory**:

```bash
cd /path/to/tweeter-gdg-1-mentor/tweeter-gdg-1
claude
```

This instance can only see:
- The tweeter-gdg-1/ directory
- Whatever context it builds from here

### Step 5: Run the Magic Bullet Prompt

In the **Mentor Mind** instance, paste the prompt from `06-magic-bullet-prompt.md`.

It will:
1. Read the tweeter-gdg-1/README.md
2. Analyze available tools (SpecSwarm, MCP servers, subagents)
3. Ask clarifying questions to fill in gaps
4. Generate the PERFECT prompt to paste into the Developer instance

### Step 6: Execute in Developer Instance

Copy the generated prompt from the Mentor Mind and paste it into the **Developer Instance**.

Then watch it:
- Plan the architecture
- Generate specifications
- Create tasks
- Build the entire application
- Test it in the browser
- Ship it

---

## What Just Happened?

Two instances. Different context windows. Different perspectives.

One sees the forest. One builds the trees.

That's **Context Stacking** in action.
