# Cold reader

Run this as the last step of the documentation page branch, and for any other text a stranger must act on. The writer's own read fills gaps from context the reader lacks, so it passes a page that a newcomer cannot follow. A cold reader has only the page.

## Procedure

1. **Write two to four tasks** the page must let its reader complete. Phrase each as the reader would, in their own words rather than the page's headings, so the task does not point at the answer. Include one task near an edge case or failure the page claims to cover. Record the correct answer for each.

2. **Start a fresh reader.** Use a subagent that starts without this conversation, such as a new general-purpose agent rather than a fork. A faster, cheaper model is fine. Give it only the prompt below, with the page text pasted in. Leave out the codebase, your intent, and the correct answers.

3. **Compare the report with the correct answers.** A wrong answer is a defect even when the reader sounds confident. For each stumble, fix the cause in the page:
   - a prerequisite that is missing or comes too late
   - a pronoun or label with an unclear referent
   - a relationship the page implies but never states
   - a needed detail buried in a long paragraph or a later section

4. **Run it again** with the same tasks if the fixes changed the page's structure. Done when every task is answered correctly and each remaining stumble is listed as a known gap.

## Prompt

```text
You are <one line describing the intended reader, e.g. "a web developer who has never used this library">.
Read only the page below. Use no outside knowledge of this project.

For each task, report:
1. Your answer, quoting the sentences you relied on.
2. Every place you hesitated, reread, or guessed. Quote the sentence and say what was unclear.
3. Anything you needed that the page did not say.

Tasks:
1. <task>
2. <task>

<page>
<page text>
</page>
```

## Limits

A model reader is a quick check, not a usability study. No published study shows how closely a model's stumbles match a real reader's. Use the reports to find problems, and keep human readers for decisions that depend on how people actually behave.
