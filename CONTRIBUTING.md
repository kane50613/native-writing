# Contributing

We welcome contributions for more languages and regional varieties. Add guidance for the language you write in, improve an example, or correct wording that sounds unnatural to you.

## Where to edit

```text
SKILL.md                       Shared process and links to language guides
references/
  languages/
    en/guide.md                English
    zh-CN/guide.md             Mainland Simplified Chinese
    zh-TW/
      guide.md                 Taiwan Mandarin
      terminology.md           Taiwan vocabulary
  formats/                     Rules shared across languages
    product-copy.md
    documentation.md
    blogs.md
  research/
    initial-samples.md         Evidence behind the initial guides
evals/                         Behavioral review cases
```

Language-specific rules belong in that language's folder. Advice that applies to every language belongs in `SKILL.md`; advice about a particular writing format belongs in `references/formats/`.

## Add a language

1. Create `references/languages/<language-tag>/guide.md`, using a language tag such as `ja`, `fr`, or `pt-BR`. Include a region when the guidance depends on it.
2. Describe the audience, sentence construction, tone, and local usage. Include original before-and-after examples for messages, product copy, and longer writing, plus a passage that should stay unchanged. Use the existing guides as starting points.
3. Put supporting sources in `sources.md` beside the guide. Record URLs, dates, access methods, what you observed, and limitations. Sample several unrelated writers. Include older original-language articles where possible, and check for revisions or translated editions.
4. Add `terminology.md` only if the vocabulary guidance needs a separate file. Link it from the guide and explain when to read it. Keep meanings and exceptions beside each term.
5. Link the guide from `SKILL.md` and the supported-language list in `README.md`. Add review cases in `evals/<language-tag>.md`, linked from [evals/README.md](evals/README.md).

Keep each guide self-contained for its audience. Reuse shared process and format references through links. Summarize sources in your own words and distinguish observed usage from your editorial recommendations.

## Before opening a pull request

Check local links and review the examples for lost facts, conditions, or changes in tone. Try the relevant [evaluation cases](evals/README.md) with an agent using the skill; report the model, prompts, outputs, and any untested behavior.

Explain what your change improves and include the supporting examples or sources. Small corrections are welcome too.
