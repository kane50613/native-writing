---
name: native-writing
description: Write, edit, or review prose in English, 台灣繁中, or 简体中文 so the reader follows it on the first read. Covers website and app copy, documentation pages and docs-site structure, PR bodies, commit messages and changesets, blog posts, books, and messages. Use when asked to write or edit copy, humanize text, remove AI voice, fix translationese, or organize documentation. Other skills use it for every piece of prose they author.
---

# Native writing

Write so the reader follows the thought on the **first read**. The reader never has to backtrack, guess what a sentence depends on, or hunt for the point. Every branch below aims at the first read, and every completion check tests it.

## Hard rules

1. **Preserve meaning.** Names, quantities, dates, conditions, negations, uncertainty, attribution, commitments, and the writer's attitude survive every edit. Add only facts the input supplies. When a claim needs a cause, measurement, source, or experience the input lacks, flag the gap briefly.
2. **Keep literals exact.** Code, commands, signatures, configuration, normative keywords such as "must", quoted interface labels, interpolation tokens, and translation keys stay as written.
3. **Local conventions win.** The user's samples and explicit preferences, a project's style guide, and a repository's templates take precedence over these references.

## Branches

Pick the branch from the request. The last column lists every file the branch reads at step 2. The tables after this one give each file's path.

| Branch | Use it for | Steps | Read at step 2 |
| --- | --- | --- | --- |
| Write or edit | Drafting or revising prose, including a few paragraphs inside a docs page. The default. | 1–4 | Language guide, the form reference from the form table below, both composition files |
| Documentation page | Writing a new README, tutorial, how-to, reference page, or help article, or rewriting most of one | 1–5 | Language guide, `documentation.md` as the form reference, both composition files. Step 5 reads `cold-reader.md`. |
| Change notes | A PR body, commit message, changeset, changelog entry, or release note | 1–4 | Language guide, `change-notes.md` as the form reference, both composition files |
| Review | Critique or alternatives, with the text left unchanged | 1, 2, 4 | The same files Write or edit would read for this text |
| Docs structure | Organizing or auditing a documentation site's navigation | The steps in `docs-structure.md`, which also define when it is done | `docs-structure.md`. Its step 2 reads `tree-test.md`. Add the language guide when you write new labels. |
| Message or reply | A chat message or an ordinary reply | 1–4 | Language guide only. Skip step 2 when the guide is already in context. |

Each output language has one guide:

| Language | Guide |
| --- | --- |
| English | [references/languages/en/guide.md](references/languages/en/guide.md) |
| 台灣繁中 | [references/languages/zh-TW/guide.md](references/languages/zh-TW/guide.md), plus the required [references/languages/zh-TW/terminology.md](references/languages/zh-TW/terminology.md) |
| 简体中文 | [references/languages/zh-CN/guide.md](references/languages/zh-CN/guide.md) |

Each form has one reference:

| Form | Reference |
| --- | --- |
| Website and app copy, interface strings, errors | [references/formats/product-copy.md](references/formats/product-copy.md) |
| Documentation pages | [references/formats/documentation.md](references/formats/documentation.md) |
| PR bodies, commit messages, changesets, changelogs, release notes | [references/formats/change-notes.md](references/formats/change-notes.md) |
| Blogs, essays, technical articles, newsletters | [references/formats/blogs.md](references/formats/blogs.md) |
| Books and manuscripts | [references/formats/books.md](references/formats/books.md) |

The composition files are [references/composition/paragraphs.md](references/composition/paragraphs.md) and [references/composition/lists.md](references/composition/lists.md). The review procedures are [references/review/cold-reader.md](references/review/cold-reader.md) and [references/review/tree-test.md](references/review/tree-test.md). The site procedure is [references/formats/docs-structure.md](references/formats/docs-structure.md).

## Steps

1. **Find the point.** Infer the reader, purpose, language, and formality from the request. For a rewrite, list the claims, qualifications, requests, and stance that must survive. For a draft, use the supplied facts and intended message. For work in a product or repository, read nearby copy, the behavior the text describes, and any template or style guide that applies under hard rule 3. Done when you can state in one sentence what the reader should understand or do. Ask only if a missing detail would change that sentence.

2. **Read the branch's files.** Read every file the branch's row lists, before writing anything. Done when you have read them all and the vocabulary, tone, and form you plan suit the reader and the actual surface.

3. **Write the thought.** Lead with the point, then give the reason or detail the reader needs next. Build each paragraph from its topic sentence, and open each sentence with something the reader already has. When a sentence is hard to follow, recover what it says and rebuild it around the action or relationship. Keep clear passages as they are. Done when each paragraph or interface string serves one purpose and every pronoun or label has a recoverable meaning.

4. **Check meaning, then the first read.** Compare the result against the input for lost and invented information under hard rule 1. Run the "Completion check" section of the form reference and the pre-delivery check in the language guide, wherever those exist. Then read only the first sentence of each paragraph. Together they should carry the piece in order. For the review branch, run these checks on the text as written and report what fails. Done when the meaning survives, the topic sentences carry the piece, and no passage forces a reread.

5. **Cold-read the page.** For the documentation page branch, follow the [cold reader](references/review/cold-reader.md) procedure. Done when a reader with no context completes every task and you have fixed each reported stumble or listed it as a known gap.

## Editorial judgment

- Give the actor and action when they matter. Keep the same name for the same thing. Use an established technical term when it is clearer than a paraphrase, and explain it for readers who need that help. Unpack newly coined labels into what actually happens.
- Let sentence length follow the thought. Keep the connective words that explain cause, sequence, conditions, or disagreement. Use paragraphs for developed ideas, lists for parallel items the reader needs to scan, and headings when they help navigate a longer piece.
- Preserve the author's warmth, frustration, humor, and degree of politeness. Express those through the situation and the writer's actual stance. Anecdotes, opinions, emotions, measurements, sources, and experience come only from the input.
- Treat punctuation, familiar idioms, repeated words, and groups of three as ordinary tools. Change them when they obstruct this passage. Follow the language guide's punctuation reference for the actual surface: a short message, developed prose, a manuscript, and an interface label need different treatment. Preserve useful sentence boundaries, relationships, and intentional rhythm. Style editing is not an AI-authorship test.
- Replace vague praise with its supported substance. If the input gives no substance, retain only what it actually establishes and flag a material gap briefly. Keep an unspecified improvement unspecified and a tentative result tentative. Fact-checking, when requested, is a separate operation from preserving meaning during an edit.

## Delivery

For a writing-only request, return the finished prose by default. Add a short note only for an unresolved ambiguity, an unsupported material claim, or a consequential editorial choice. For the review branch, return the findings instead. During implementation, edit the requested product copy or documentation and follow the parent task's delivery requirements. Keep the editorial checklist out of the deliverable.

For a requested voice that these references do not cover, follow the [research method in CONTRIBUTING.md](CONTRIBUTING.md#research-a-language-or-regional-variety) to gather suitable samples. Routine writing does not require browsing.
