# Lists or prose

Read this before drafting, and again before turning prose into a list or a list into prose. Major style guides recommend lists because readers scan web pages. Critics of bullet-heavy writing point out that a list hides how its items relate. Both are right about different content, so decide by the relationship between the items. For 台灣繁中, also read [the zh-TW composition reference](../languages/zh-TW/composition.md), which covers enumeration commas and one-item-per-line notices.

## Decide by the relationship

Use a list when the items are parallel. Options, independent facts, conditions that each lead to the same outcome, and things to check all qualify. The connectives a list drops between parallel items are "and", "also", and "or", so the reader loses nothing. Use a numbered list when the order matters, as in a procedure or a ranking.

Write prose when the items depend on each other. Cause, condition, contrast, and trade-off live in words like "because", "unless", "but", and "so". A list drops those words, and the reader has to rebuild the argument. A narrative also forces the writer to decide what matters more than what.

Mixed content takes both forms. A sentence states the relationship, a list holds the parallel items, and a sentence after the list covers the exception.

## Shape the list

- Introduce the list with a complete sentence, unless the heading directly above already says what the list contains.
- Keep two to seven items, short enough that the reader sees two or three at a glance.
- Give every item the same grammatical shape, such as all noun phrases or all sentences starting with a verb.
- Keep each item to one sentence. An item that needs several sentences is a paragraph or a subsection.
- Use a list only for two or more items. Set off a single item some other way.

## Example

Input: “Takumi retries a request if the connection fails. Takumi also retries if the request times out. It also retries on HTTP 408, 429, 500, 502, 503, and 504.”

Rewrite: “Takumi retries a request when any of these happens:

- The connection fails.
- The request times out.
- The server responds with HTTP 408, 429, 500, 502, 503, or 504.”

The three conditions lead to the same outcome, so the "also" between them carried no information. A rule like “Takumi waits for `Retry-After`, unless it asks for more than one second” stays a sentence, because "unless" is the content.

## Sources

- Google, [Lists](https://developers.google.com/style/lists): lists suit sequential information or a simple collection of items, introduced by a complete sentence.
- Microsoft, [Lists](https://learn.microsoft.com/en-us/style-guide/scannable-content/lists): two to seven items, short and consistent in structure.
- GOV.UK, [A to Z style guide, bullet points](https://guidance.publishing.service.gov.uk/writing-to-gov-uk-standards/style-guides/a-to-z-style-guide/): always use a lead-in line, one sentence per bullet.
- Federal plain language guidelines, [use lists](https://github.com/GSA/plainlanguage.gov/blob/main/_pages/guidelines/organize/use-lists.md): lists suit items, conditions, and exceptions.
- Jakob Nielsen, [How Users Read on the Web](https://www.nngroup.com/articles/how-users-read-on-the-web/) (1997): most users scanned, and a scannable layout measured 47% better usability.
- Edward Tufte, [The Cognitive Style of PowerPoint](https://www.edwardtufte.com/notebook/new-edition-of-the-cognitive-style-of-powerpoint/) (2003): bullet outlines let the presenter skip tying the information together.
- Jeff Bezos, 2004 email on narrative memos, [as quoted by CNBC](https://www.cnbc.com/2018/04/23/what-jeff-bezos-learned-from-requiring-6-page-memos-at-amazon.html): narrative structure forces better thought about what is more important than what.
