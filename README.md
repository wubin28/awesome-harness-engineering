# Awesome Harness Engineering [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of KOLs' content on harness engineering: the practice of shaping the environment around AI agents so they can work reliably.

Harness engineering sits at the intersection of context engineering, evaluation, observability, orchestration, safe autonomy, and software architecture. This list focuses on content by key opinion leaders — articles, podcasts, videos, and other formats — that make agents more dependable in real workflows, especially long-running coding and research tasks.

## Contents

- [KOLs' Content for Coding Agent Users](#kols-content-for-coding-agent-users)
- [KOLs' Content for Coding Agent Builders](#kols-content-for-coding-agent-builders)
- [Contributing](#contributing)
- [License](#license)

## KOLs' Content for Coding Agent Users

- 2026-04-07-harness-user-blog-redhat [Harness engineering: Structured workflows for AI-assisted development](https://developers.redhat.com/articles/2026/04/07/harness-engineering-structured-workflows-ai-assisted-development) - For developers frustrated by unpredictable AI coding agents that hallucinate file paths and invent non-existent APIs, this article introduces a two-phase harness workflow: a repository impact map built from LSP/MCP-grounded symbol analysis that a human reviews before any tasks are created, followed by structured task templates with real file paths, symbol references, and acceptance criteria — constraining the solution space so that structured input reliably produces targeted, consistent code output.

- 2026-04-02-harness-user-tw-blog [Harness engineering for coding agent users](https://martinfowler.com/articles/harness-engineering.html) - For developers and engineering teams struggling with unreliable AI coding agents that require excessive manual review, this article introduces "harness engineering for coding agent users" — a systematic approach of combining feedforward guides (rules, specs, language servers) and feedback sensors (linters, tests, AI reviewers) across computational and inferential dimensions to increase agent accuracy, enable self-correction, and reduce supervision toil.

- 2026-03-12-harness-user-blog-humanlayer [Skill Issue: Harness Engineering for Coding Agents](https://www.humanlayer.dev/blog/skill-issue-harness-engineering-for-coding-agents) - For developers blaming model quality for repeated coding agent failures, this article reframes poor output as a configuration problem and walks through the highest-leverage harness levers — AGENTS.md, MCP servers, skills, sub-agents, hooks, and back-pressure — with concrete patterns proven in complex enterprise brownfield codebases.

- 2026-02-17-harness-user-tw-blog [Harness Engineering - first thoughts](https://martinfowler.com/articles/exploring-gen-ai/harness-engineering-memo.html) - For software engineering leaders wondering whether systematic harness design is worth the effort, this memo reflects on OpenAI's five-month experiment building one million lines of agent-generated code, examining how deterministic linters, architectural constraints, and iterative garbage collection collectively made the codebase maintainable — and raising open questions about greenfield versus brownfield applicability.

- 2026-02-11-harness-user-blog-openai [Harness engineering: leveraging Codex in an agent-first world](https://openai.com/index/harness-engineering/) - For engineering teams aiming to build and maintain large codebases with AI agents, this article documents OpenAI's five-month experiment producing one million lines of zero-manually-written code using Codex, describing the full harness: structured repository knowledge bases, custom architectural linters, browser and observability tooling, agent-to-agent review loops, and continuous garbage-collection agents that fight entropy.

- 2026-02-05-harness-user-blog-hashimoto [My AI Adoption Journey](https://mitchellh.com/writing/my-ai-adoption-journey) - For experienced developers skeptical of AI coding tools or stuck in early adoption frustration, this personal account by Mitchell Hashimoto traces a pragmatic six-step journey from chatbot experiments to "harness engineering" — the practice of iteratively encoding agent failure modes into AGENTS.md files and automated verification tools so mistakes never repeat. This is the first time the term "harness engineering" has been formally coined on a blog.

## KOLs' Content for Coding Agent Builders

- 2026-03-24-harness-builder-blog-anthropic [Harness design for long-running application development](https://www.anthropic.com/engineering/harness-design-long-running-apps) - For AI engineers hitting quality ceilings with single-agent long-running coding systems, this article presents a GAN-inspired three-agent architecture (planner, generator, evaluator) that uses structured sprint contracts and browser-driven QA to produce richer full-stack applications with fewer stub features and missed requirements.

- 2026-03-10-harness-builder-blog-langchain [The Anatomy of an Agent Harness](https://blog.langchain.com/the-anatomy-of-an-agent-harness/) - For engineers building autonomous agents who want a principled framework for harness design, this article derives each core harness component — filesystems, bash execution, sandboxes, context compaction, skills, planning loops, and sub-agents — by working backwards from specific model limitations, showing how harness engineering converts intelligence into reliable, long-horizon work.

- 2026-03-03-harness-builder-blog-inngest [Your Agent Needs a Harness, Not a Framework](https://www.inngest.com/blog/your-agent-needs-a-harness-not-a-framework) - For developers drowning in custom retry logic, state persistence, and event routing for their AI agents, this article argues that durable event-driven infrastructure already solves these problems and demonstrates the point with Utah — a production-quality conversational agent built on Inngest without any AI framework, featuring sub-agent delegation, singleton concurrency, and two-tier context pruning.

- 2025-11-26-harness-builder-blog-anthropic [Effective harnesses for long-running agents](https://www.anthropic.com/engineering/effective-harnesses-for-long-running-agents) - For developers whose AI coding agents lose coherence or declare early victory on multi-session tasks, this article presents Anthropic's two-agent harness solution: an initializer that scaffolds a feature list, init.sh script, and progress file, plus a coding agent that works incrementally, verifies features end-to-end via browser automation, and leaves structured git artifacts for the next session.

- 2024-12-19-harness-builder-blog-anthropic [Building Effective AI Agents](https://www.anthropic.com/engineering/building-effective-agents) - For developers tempted to reach for complex frameworks before understanding the fundamentals, this article from Anthropic establishes the composable building blocks of agentic systems — augmented LLMs, prompt chaining, routing, parallelization, orchestrator-workers, and evaluator-optimizers — with practical guidance on when agents are appropriate and how to design tools as carefully as prompts.

## Contributing

Contributions are welcome. Please prefer resources that are:

- Specific about how agents are constrained, evaluated, resumed, observed, or orchestrated
- Original implementations, primary-source articles, or high-signal technical write-ups
- Useful to practitioners building real harnesses instead of generic AI commentary

If two links say the same thing, prefer the more primary, practical, and implementation-oriented one.

See [CONTRIBUTING.md](./CONTRIBUTING.md) for contribution guidelines and the preferred entry format.

## License

[MIT](./LICENSE)
