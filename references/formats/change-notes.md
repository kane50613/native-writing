# Change notes

Use this for PR bodies, commit messages, changesets, and release notes. Each has a different reader. A reviewer reads the PR body to decide whether the change is right. A maintainer reads the commit history later to learn what changed and why. A user scans the changeset or release note to learn what an upgrade does to them. A repository's own template or conventions take precedence over the defaults below.

## What every note leaves out

Each sentence must change what its reader does or understands. Delete a sentence outright, rather than shortening it, when it states:

- a fact the reader can see in the diff
- a caveat about a case nobody will hit
- a claim about how good the change is
- test or CI results, which CI already reports
- a measurement the reader cannot act on
- a rejected alternative or the story of finding the problem
- the reasoning behind a decision no reviewer is being asked to make
- a limitation the code's own docs already record

## PR body

Unless the repository has a template, the body is an optional issue line and two sections:

```markdown
Fixes #<issue>

## Why
<the defect or need, stated once>

## What
<what the code does now, stated once>
```

Open with `Fixes #<issue>` only when the work came from an issue, so the merge closes it. Keep the number out of the prose below.

**Why** states the defect that existed or the need the change meets. **What** states what the code does now, not which files changed. Write two sentences in each section, each under about 25 words. A diff over about 500 lines earns a third. Keep one paragraph under each heading. When the change has several independent parts, give each part one bullet of one sentence. More than about four parts suggests the PR should be split.

Add at most one more fact, and only one that changes how someone reviews. A non-obvious invariant, a deliberate omission, or a risk to look at qualifies. Write it as one more sentence at the end of the section it belongs to, so each heading still has one paragraph.

Write each paragraph as one line. GitHub renders every line break in a PR body, so hard-wrapped text shows up as ragged short lines.

Short sentences can still be hard to read. Nested noun phrases make a reviewer parse the sentence twice:

> A forced break between some content and an out-of-flow box that follows it left the box's static position at the end of the page before the break, where Blink's `HandleOutOfFlowPositioned` breaks before the box.

Name the actor and the event, then the consequence:

> A forced break before an out-of-flow box left the box's static position at the end of the earlier page. Blink's `HandleOutOfFlowPositioned` breaks before the box instead.

## Commit message

Match the subject style in the repository's recent history. The subject names the outcome a user sees, not the mechanism: "Support `display: table`", not "Lay out tables on the grid algorithm". A body, when the change needs one, gives the reason the diff cannot show.

## Changeset and release note

Match a neighboring entry's front matter, filename, and heading style first, because each tool has its own format. Write one heading stating the outcome a user gets. Follow it with at most one short paragraph on what changed and what users see, naming the types, functions, and errors they touch. Rationale, investigation, and alternatives belong in the PR body.

## Completion check

Count the words you wrote in the PR body, leaving out the issue line and anything a bot generated. Two sections of two sentences plus one extra fact come to about 120 words. A longer body needs a cut from the list above, or a split into separate PRs. Check that the body has only the Why and What headings unless the repository's template asks for more. Read Why and What as a reviewer who has not seen the diff. Each should make sense on the first read.
