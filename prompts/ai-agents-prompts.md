# 🤖 AI Agent Prompts

Prompts for using GPT as an autonomous agent, designing your own agents, and getting the most out of coding agents (like Claude Code, Copilot, or Cursor).

## 1. Multi-Step Task Agent

```text
Act as an agent completing this task step by step.

Task: [DESCRIBE THE TASK]

Please:
1. Break the task into a numbered plan before starting
2. Work through the plan one step at a time
3. After each step, briefly say what you did and what's next
4. Stop and ask me if you're missing information you need to continue
5. Summarize the final result at the end
```

## 2. Design a Custom AI Agent

```text
Help me design an AI agent for this purpose: [DESCRIBE WHAT THE AGENT SHOULD DO]

Please define:
1. The agent's goal in one sentence
2. What tools/data it would need access to (e.g. web search, a database, an API)
3. Its step-by-step decision process (how it decides what to do next)
4. What it should NOT do (guardrails/limits)
5. An example scenario showing how it would handle a typical request
```

## 3. Write a System Prompt for an Agent

```text
Write a system prompt for an AI agent with this role: [DESCRIBE THE ROLE, e.g. customer support agent, research assistant]

Please include:
1. A clear description of its role and goal
2. Its tone/personality
3. What it should always do
4. What it should never do
5. How it should handle a request it can't fulfill

Keep it clear and specific, not vague.
```

## 4. Plan a Coding Task for an AI Coding Agent

```text
I want to give this task to an AI coding agent (like Claude Code, Copilot, or Cursor). Help me write clear instructions for it.

Task: [DESCRIBE WHAT YOU WANT BUILT OR FIXED]
Relevant files/context: [DESCRIBE OR PASTE RELEVANT CODE/STRUCTURE]

Please:
1. Rewrite my task as a clear, specific instruction the agent can follow
2. List any missing details the agent will need
3. Suggest constraints to include (e.g. "don't modify X file", "use existing style")
4. Suggest how I should verify the agent's work when it's done
```

## 5. Review an AI Agent's Output

```text
An AI coding agent made these changes. Help me review them before I accept them.

Changes made:
[PASTE THE DIFF, SUMMARY, OR DESCRIPTION OF CHANGES]

Please:
1. Summarize what actually changed in plain terms
2. Flag anything risky, unexpected, or outside the scope of what I asked for
3. Point out anything that looks untested or incomplete
4. Suggest what I should test manually before merging/accepting
```
