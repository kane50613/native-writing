# native-writing

An agent skill for natural writing across languages and regions.

Write website and app copy, documentation, blog posts, and everyday messages in language that fits the reader. Keep the facts, explain the thought, and preserve the writer's voice.

## Install

With the [skills CLI](https://github.com/vercel-labs/skills):

```sh
npx skills add kane50613/native-writing --skill native-writing
```

Choose your agent and installation scope when prompted. Add `--global` to make the skill available across projects.

You can also copy this repository's `SKILL.md` and `references/` into a `native-writing` folder in your agent's skills directory. Both are required.

## Use

Ask your agent to use `native-writing`, then provide the task, audience, and source material. For agents that support dollar-sign skill mentions:

```text
Use $native-writing to edit this README for developers trying the library
for the first time. Keep the prerequisites and limitations.
```

```text
用 $native-writing 改寫這個 app 的錯誤訊息，給台灣使用者看。
請先確認實際的錯誤原因，以及使用者能做什麼。
```

```text
用 $native-writing 修改这篇技术博客，面向刚接触这个工具的开发者。
保留测试条件和作者的口吻。
```

The skill also applies to user-facing copy while an agent builds a website or app. Routine writing does not require browsing or a particular browser tool.

## Languages and regions

| Reference | Current scope |
| --- | --- |
| [English](references/english.md) | General English, adapted to the audience and the writer's samples |
| [台灣繁中](references/zh-tw.md) | Taiwan Mandarin, with a contextual [terminology guide](references/taiwan-terms.md) |
| [简体中文](references/zh-cn.md) | Mainland Chinese usage by default, adjusted when another region is specified |

The project is designed to grow through language and regional references. These are the three currently included. Regional guidance covers sentence construction, tone, and terminology, beyond converting characters or substituting words.

## What it pays attention to

- **Meaning:** preserve conditions, uncertainty, numbers, attribution, and commitments.
- **Reader and surface:** a button, an error message, a tutorial, and a personal essay have different jobs.
- **Local usage:** choose vocabulary in context and preserve real interface labels and proper names.
- **Voice:** retain useful humor, courtesy, frustration, and distinctive phrasing. Leave clear passages alone.
- **Evidence:** replace vague claims with supported substance, and flag material gaps without inventing details.

For example:

> The cache delivered a significant performance enhancement, reducing startup from 800 ms to 500 ms in one local test, although its production impact has yet to be validated.

Becomes:

> The cache cut startup from 800 ms to 500 ms in one local test. We haven't tested it in production yet.

The measurement and its limit both survive. The reference files include original exercises for each language and writing format.

Punctuation follows the passage. Periods are a useful default, and semicolons remain available when they help. The skill makes no claim to detect AI authorship or guarantee an AI detector score.

## Structure

```text
SKILL.md                         Shared process and reference routing
references/
  english.md                     English prose
  zh-tw.md                       Taiwan Mandarin prose
  zh-cn.md                       Simplified Chinese prose
  taiwan-terms.md                 Contextual Taiwan vocabulary
  product-copy.md                 Website and app copy
  documentation.md               Documentation and technical documents
  blogs.md                       Blogs and essays
  community-research.md          Sources, observations, and limitations
evals/
  README.md                      Behavioral review cases and rubric
```

The agent reads the shared process, the relevant language reference, and any needed writing-format reference. Research notes are available when reviewing evidence or studying another voice.

## Research and contributions

The guidance draws on a small sample of communities, older blogs, documentation, and product pages. The [research notes](references/community-research.md) distinguish directly read pages from indexed excerpts, record access limitations, and separate observations from editorial decisions. An old publication date is not proof that today's page is unchanged or entirely human-written.

Contributions for additional languages and regions are welcome. See [CONTRIBUTING.md](CONTRIBUTING.md) for the evidence and examples to include, and [evals/README.md](evals/README.md) for review cases.

## License

[MIT](LICENSE). Linked third-party writing belongs to its respective authors. Editing exercises in this repository are original examples.
