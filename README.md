# Project Interviewer

`project-interviewer` is a Codex skill that interviews someone about a project idea until the intended outcome is genuinely clear.

It is built for the moment before planning, specs, architecture, or execution, when someone says "I want to build something" but the real shape of that thing is still fuzzy.

## Why This Exists

Most project conversations jump to solutions too early.

Someone says:

- "I want an AI app"
- "I think I need a SaaS"
- "I want to build a tool for my team"
- "I have an idea, but I do not know how to frame it yet"

What they usually need first is not a stack recommendation or roadmap. They need a strong interviewer who can keep asking until the goal is specific, grounded, and emotionally true.

This skill is designed to do that.

## What The Skill Does

The skill:

- stays in discovery mode before planning
- asks adaptive follow-up questions instead of running a rigid questionnaire
- separates the user's actual intent from their first proposed solution
- pressure-tests vague words like "simple", "MVP", "premium", or "AI-powered"
- keeps interviewing until confidence is earned, not assumed
- produces a clean handoff with confirmed facts, working inferences, and open edges

## What "95% Confidence" Means

The stopping rule is intentionally strict.

The skill should not stop interviewing just because the conversation has been long. It should stop only when the project is clear enough that two competent builders would likely interpret the first version the same way.

That means the interview should uncover:

- the desired end state
- who the project is for
- what problem or desire is driving it
- what matters in version one
- what constraints and deal-breakers exist
- what is confirmed by the user versus inferred by the model

## Good Use Cases

This skill is designed to work across many project types:

- products and SaaS ideas
- internal tools and workflows
- creative projects
- research projects
- learning projects
- service businesses and consulting offers

## Example Prompts

```text
Use $project-interviewer to interview me about a product idea until you are 95% confident about what I actually want.
```

```text
Use $project-interviewer to help me clarify an internal tool idea for my team. Keep asking questions until the first version is concrete.
```

```text
Use $project-interviewer to interview me about a creative project. Do not push startup language onto it.
```

## How It Works

The skill follows a simple pattern:

1. Anchor the idea in the user's own words.
2. Expand only into dimensions that still matter.
3. Pressure-test fuzzy language and contradictions.
4. Separate desired outcomes from proposed solutions.
5. Re-state the current understanding and invite correction.
6. Stop only when the remaining unknowns would not materially change the next step.

## Output Shape

When the interview is complete, the skill produces:

- `What You Actually Want`
- `Confirmed Facts`
- `Working Inferences`
- `Open Edges`
- `Recommended Next Step`

## Repository Structure

- [`project-interviewer/SKILL.md`](./project-interviewer/SKILL.md): main skill instructions
- [`project-interviewer/references/interview-map.md`](./project-interviewer/references/interview-map.md): adaptive interview checklist and follow-up patterns
- [`project-interviewer/agents/openai.yaml`](./project-interviewer/agents/openai.yaml): UI metadata

## Installing The Skill

Copy the `project-interviewer` folder into your Codex skills directory, typically:

```text
${CODEX_HOME:-~/.codex}/skills/project-interviewer
```

If you are developing locally, you can also keep the skill in a workspace and invoke it by path when needed.

## Design Principles

- Do not mistake a feature list for a clear project.
- Do not substitute best practices for user intent.
- Do not assume business framing fits every project.
- Do not stop at "good enough" if the core ambiguity is still unresolved.
- Do not interrogate forever once clarity is real.

## License

MIT
