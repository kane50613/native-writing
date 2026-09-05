# Contributing

Help agents write clearly for a particular audience. Useful contributions include a language or regional reference, a better original example, or a correction supported by actual usage.

## Add a language or region

1. Describe the audience and register the reference covers. A writing system alone does not identify a region or community.
2. Read several unrelated writers in the original language. Match the sources to the intended work: include blogs and documentation for long-form writing, and actual product surfaces for interface copy. Older articles can provide useful baselines. Check revision dates and translated editions.
3. Record URLs, displayed dates, access methods, and the passages or sections inspected in `references/community-research.md`. Distinguish your observations from the guidance you recommend. Record inaccessible sources as gaps.
4. Add a focused language reference under `references/`. Explain sentence construction, register, and context-sensitive terminology. Include original examples that preserve facts and examples that should stay unchanged.
5. Link the reference from `SKILL.md`, update the language table in `README.md`, and add relevant behavioral cases under `evals/`.

Keep shared editing principles in `SKILL.md` and form-specific guidance in the existing form references. A new language normally needs a reference file, not another skill or a duplicate copy of the shared process.

Use short attributed excerpts only when necessary. Prefer your own summaries and exercises. Public availability does not grant permission to copy whole posts. Do not infer someone's nationality or authorship from the platform they use.

## Review a change

Check that each local Markdown link resolves and that the skill frontmatter still identifies `native-writing`. Read every changed instruction with its surrounding reference: a vocabulary preference must not alter a quotation, a literal UI label, or a technical meaning.

Run the relevant cases in [evals/README.md](evals/README.md) with an agent that can load the skill. Record the agent/model, date, prompt, output, and observed failures in the pull request. Review meaning and usability before stylistic preferences. Mark untested behavior explicitly.

A pull request should explain the concrete problem, resulting behavior, supporting evidence, and validation performed. Include a small reproduction when fixing a writing failure. Avoid adding a universal ban to fix a single awkward sentence.
