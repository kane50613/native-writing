# Docs structure

Use this for the docs structure branch, which organizes or audits a documentation site's navigation. Single pages follow the [documentation](documentation.md) reference instead. Readers find things in two ways. They **pull** what they came for by following labels, groups, and search. The docs **push** what they should see, such as the core model and the common mistakes, through an ordered path and links. A good structure serves both.

## Steps

1. **Inventory the site.** List every page with its title, the reader's job it serves (learn, do a task, look something up, or understand), its audience, its length, and how many other pages link to it. Record the navigation groups as the reader sees them. Done when every page appears once with all five facts.

2. **Run a baseline tree test.** Follow the [tree test](../review/tree-test.md) procedure on the current navigation. Done when each task has a recorded first click, final location, and result.

3. **Diagnose.** Check the inventory and the test results against the rules below. Done when each finding cites a failed task or a number from the inventory.

4. **Propose one change.** Pick the finding with the most failed tasks behind it. Describe the moves, the new labels, a redirect for every changed URL, and the tasks the change should fix. Done when someone else could apply the proposal without asking you anything.

5. **Retest after the change lands.** Run the same tasks again. Done when the targeted tasks pass and none of the others regressed.

Change the structure one group at a time. Building a complete framework of empty sections first produces structure without content. Let the top-level shape emerge from the improved pages.

## Rules

**Group by the reader's goal.** Directory layout and package boundaries are the maintainer's model. Split the top level by package only when the packages serve different readers, such as people generating images and people generating PDFs. Content that several packages share, such as styling or fonts, needs one home that each package's pages link to. Shared content filed under one package stays invisible to the readers of the others.

**Keep groups small.** A group of more than about seven items is hard to scan. Split it by task, and keep the reader's jobs apart. A group that mixes tutorials, reference pages, and troubleshooting asks the reader to sort it.

**Make labels predict their pages.** A reader chooses a link by guessing its content from the label. Name pages by task or subject, and give no two items the same label. Two pages called "Reference" in different sections force the reader to open both.

**Split pages that hide tasks.** The navigation shows only page titles. A long page that covers several tasks hides all but the first from a reader scanning the sidebar. Split it so each task gets a title.

**Give learners an ordered path.** Keep a short sequence of getting-started pages, each ending with a link to the next. Keep that path separate from lookup material. Next.js opens with eighteen numbered getting-started pages before its guides and API reference. React separates its Learn chapters from its Reference.

**Give the core model one page.** Facts about how the system works, such as how it differs from a browser, tend to end up scattered across pages as warnings. Collect them on one explanation page. Link it from the getting-started path and from every warning that depends on it.

**Expect readers to arrive anywhere.** A reader who lands on a page from search should find its prerequisites linked from that page. Check this on the pages with the most inbound search traffic or links.

## Framework notes

Fumadocs requires each page URL to appear only once in the page tree, and it renders root folders as tabs. A page shared across tabs lives in one place. Other tabs reach it through a link item such as `[Styling](/docs/styling)` in `meta.json`. Check how the sidebar highlights the active page after adding one.

## Sources

- Diátaxis, [How to use Diátaxis](https://diataxis.fr/how-to-use-diataxis/): improve one step at a time and let structure emerge, rather than creating empty sections.
- Nielsen Norman Group, [Tree Testing](https://www.nngroup.com/articles/tree-testing/) and [Information Scent](https://www.nngroup.com/articles/information-scent/).
- Mark Baker, [*Every Page is Page One*](https://xmlpress.net/publications/eppo/) (XML Press, 2013).
- Next.js, [getting-started pages](https://github.com/vercel/next.js/tree/canary/docs/01-app/01-getting-started). React, [Learn sidebar](https://github.com/reactjs/react.dev/blob/main/src/sidebarLearn.json).
- Fumadocs, [page conventions](https://github.com/fuma-nama/fumadocs/blob/dev/apps/docs/content/docs/headless/page-conventions.mdx).
