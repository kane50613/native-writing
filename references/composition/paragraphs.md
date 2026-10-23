# Paragraphs

Read this before drafting the first paragraph of any prose longer than a message. It covers where a paragraph starts and ends and how its sentences connect. The guidance comes from English-language style guides and research. For Chinese, the language guide's paragraph advice takes precedence where the two differ.

## One topic, stated first

A paragraph holds one topic. Start a new paragraph when the topic changes, when you turn to a contrast, when the reader needs a pause, or when an introduction ends.

Open the paragraph with its point. Busy readers often read only first sentences, so the opening sentence should tell them what the rest supports. A reader who skims only the topic sentences should still get the piece's general meaning. Move any sentence that does not support the topic sentence to the paragraph it belongs to.

## Length follows the topic

Most explanatory paragraphs run three to five sentences. Readers tend to avoid paragraphs of more than about seven sentences, and plain language guidelines suggest at most about 150 words. Vary the length with the material, since paragraphs of uniform size read as choppy.

A one-sentence paragraph works for a transition between sections, a sentence that introduces a code block or list, or a deliberate point of emphasis. A run of one- and two-sentence paragraphs is a symptom instead. Sentences that share a topic belong in one paragraph, joined by the words that state how they relate.

## Connect each sentence to the last

Open each sentence with information the reader already has, and end it with the new information. Readers stress the end of a sentence, so the new point belongs there. Keep the grammatical subject close to its verb, and give context before asking the reader to take in something new.

Three kinds of transition link sentences and paragraphs:

- **Pointing words** such as "this", "that", and "these" refer to something already mentioned.
- **Echo links** repeat a key word or idea from the previous sentence.
- **Explicit connectives** such as "however", "therefore", and "also" state the relationship.

Writers who know the material well tend to omit transitions, because the relationship is obvious to them. Readers rely on them. Words like "because", "unless", "but", "so", and "then" carry cause, condition, contrast, and sequence. Deleting them to shorten a paragraph deletes information.

Keep one name for one thing. Swapping in a synonym for variety makes the reader ask whether a second thing has appeared.

## Example

Input: “GET and HEAD requests make up to three attempts. The waits are 100 ms, then 200 ms. A `Retry-After` header can extend a wait up to one second. A longer `Retry-After` returns the error without retrying.”

Rewrite: “Takumi retries a failed GET or HEAD request up to two times. Before each retry it waits longer, first 100 ms and then 200 ms. A `Retry-After` header can extend that wait to at most one second. If the server asks for a longer wait, Takumi returns the error without retrying.”

The second sentence of the input opens with “The waits”, which the first sentence never mentioned. In the rewrite, “each retry” echoes the first sentence, and the new numbers land at the end. The last sentence names the condition with “If”. The rewrite keeps every number and condition, and adds no reason for the one-second limit, because the input gives none.

## Sources

- George D. Gopen and Judith A. Swan, “The Science of Scientific Writing”, *American Scientist* 78(6), 1990. [Summary of its principles](https://wstomv.win.tue.nl/quotes/science-of-scientific-writing.html).
- Google, [Technical Writing One: Paragraphs](https://developers.google.com/tech-writing/one/paragraphs).
- Purdue OWL, [On Paragraphs](https://owl.purdue.edu/owl/general_writing/academic_writing/paragraphs_and_paragraphing/index.html).
- William Strunk Jr., *The Elements of Style*, rules 8 and 9 ([Project Gutenberg](https://www.gutenberg.org/files/37134/37134-h/37134-h.htm)). Strunk discourages one-sentence paragraphs except for transitions. Web-oriented guides accept them occasionally.
- Federal plain language guidelines, archived by GSA: [write short paragraphs](https://github.com/GSA/plainlanguage.gov/blob/main/_pages/guidelines/concise/write-short-paragraphs.md), [have a topic sentence](https://github.com/GSA/plainlanguage.gov/blob/main/_pages/guidelines/organize/have-a-topic-sentence.md), [use transition words](https://github.com/GSA/plainlanguage.gov/blob/main/_pages/guidelines/organize/use-transition-words.md). The transition types come from Bryan A. Garner, *Legal Writing in Plain English* (2001).
- Jack Selzer, [“Certain Cohesion Elements and the Readability of Technical Paragraphs”](https://pure.psu.edu/en/publications/certain-cohesion-elements-and-the-readability-of-technical-paragr/) (1982). Breaking the old-to-new order and replacing repeated words with synonyms made technical paragraphs harder to read.
