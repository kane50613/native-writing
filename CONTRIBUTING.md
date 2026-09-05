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
3. Put supporting sources in `sources.md` beside the guide, using the research process below.
4. Add `terminology.md` only if the vocabulary guidance needs a separate file. Link it from the guide and explain when to read it. Keep meanings and exceptions beside each term.
5. Link the guide from `SKILL.md` and the supported-language list in `README.md`. Add review cases in `evals/<language-tag>.md`, linked from [evals/README.md](evals/README.md).

Keep each guide self-contained for its audience. Reuse shared process and format references through links.

## Research a language or regional variety

Start with a narrow question you can investigate, such as how local help articles explain errors or how writers connect ideas in personal essays. A useful first contribution can cover one recurring problem; it does not need to describe an entire language.

### 1. Find writing that matches the task

Search in the target language, using terms local readers would search for. Start with several unrelated writers across more than one site. Expand the sample when a proposed rule rests on one author's habit or when writers disagree.

| Writing task | Useful samples | What to compare |
| --- | --- | --- |
| Everyday messages | Local forums, community discussions, public social posts | Requests, disagreement, politeness, emotion |
| Blogs and essays | Personal blogs, independent publications | Openings, paragraph flow, examples, endings |
| Documentation | Help centers, tutorials, technical references | Prerequisites, steps, conditions, terminology |
| Website and app copy | Local product pages and visible interface states | Labels, calls to action, errors, recovery instructions |

Search for actual topics people write about, rather than only advice on “writing naturally.” Queries can combine a local topic with `site:<community-domain>` or `before:2022`. Search operators help discovery; verify dates and context on the page itself.

For older prose, prefer original-language articles published before 2022 and check for later revisions or automatic translations. For current interface terms, inspect current products. An old date alone does not prove the displayed text is unchanged or human-written. Note gaps in genre, region, and audience coverage.

### 2. Read enough context

Open the original page in a browser when possible. Read the surrounding paragraphs or discussion; for product copy, inspect the state and action the text describes. Any browser or research tool is fine.

If access fails, try an available public archive, search-index excerpt, or public repost. Record which you used and analyze only what you could see. After the original and a reasonable public alternative fail, use another source. Avoid spending the research session trying to get through a login wall.

Separate the author's prose from quotations, advertising, code, navigation, translations, and generated summaries. If counting punctuation, record the sections included and exclusions. A semicolon in code says nothing about its use in prose.

### 3. Turn observations into scoped guidance

For each useful passage, ask what helps the reader follow it: word order, explicit relationships, omitted subjects, concrete details, stable terms, or an appropriate degree of formality. Look for counterexamples before making a general recommendation.

Keep three things separate in your notes:

- **Observation:** what happens in the passages you read.
- **Recommendation:** what an agent should do in a specified context.
- **Limit:** where that recommendation may not apply or where evidence is missing.

For example, finding few semicolons in several essays can support periods as a default for similar prose. It does not support banning semicolons across a language. Likewise, a forum's slang may fit that community but sound wrong in an app's error message.

Compare regional vocabulary in similar contexts, ideally equivalent product surfaces or documents on the same topic. Record each term's meaning and exceptions. Platform membership and popularity do not establish nationality, writing quality, or a universal local preference.

### 4. Record sources so someone else can review them

Use this entry format in the language folder's `sources.md`:

```text
Source: title and URL
Context: language/region, intended audience, writing format
Dates: publication, visible revision, and date accessed; unknown where unavailable
Access: original page, archive, indexed excerpt, or repost; sections inspected
Observation: the specific writing choice and what it accomplishes
Recommendation: proposed guidance and when it applies
Limits: counterexamples, missing context, or uncertain provenance
```

Summarize in your own words. Include only short, attributed excerpts when needed to explain a finding. The [initial research notes](references/research/initial-samples.md) show completed observations and access limitations.

### 5. Try the guidance on fresh examples

Write original editing exercises that test the proposed rule. Include a straightforward case, an exception, and an already-clear passage that should stay unchanged. Preserve facts and voice in the intended rewrite; keep community quotations separate from your own examples.

Try the guide on additional text beyond the examples used to write it. Compare outputs with and without the proposed guidance under the same prompt and model when practical. Check meaning first, then ask a fluent reader familiar with the audience whether the result sounds natural for that setting.

Record failures and narrow the guidance accordingly. One successful rewrite is useful evidence, not proof that a rule works for a whole language. See [evaluation cases](evals/README.md) for checks you can reuse.

## Before opening a pull request

Check local links and review the examples for lost facts, conditions, or changes in tone. Try the relevant [evaluation cases](evals/README.md) with an agent using the skill; report the model, prompts, outputs, and any untested behavior.

Explain what your change improves and include the supporting examples or sources. Small corrections are welcome too.
