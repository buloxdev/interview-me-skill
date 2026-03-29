# Project Interviewer

`project-interviewer` is a Codex skill for interviewing someone about a new project until their actual intent is clear.

It is designed to:

- stay in discovery mode before planning
- separate user intent from proposed solutions
- keep asking adaptive follow-up questions until confidence is earned
- summarize confirmed facts separately from working inferences

## What It Is For

This skill works across many project types, including:

- products and SaaS ideas
- internal tools
- research projects
- service offers
- creative projects

## Contents

- [`project-interviewer/SKILL.md`](./project-interviewer/SKILL.md): the main skill instructions
- [`project-interviewer/references/interview-map.md`](./project-interviewer/references/interview-map.md): the adaptive interview checklist
- [`project-interviewer/agents/openai.yaml`](./project-interviewer/agents/openai.yaml): UI metadata for the skill

## Usage

Use the skill explicitly:

```text
Use $project-interviewer to interview me about a project idea until you are 95% confident about what I actually want.
```

## License

MIT
