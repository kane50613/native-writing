# Tree test

Run this in the docs structure branch, before and after each change. A tree test shows the reader only the navigation labels, with no page content, and asks where they would look for something. It measures whether the labels and grouping lead to the right page.

## Procedure

1. **Extract the tree.** Write out the navigation as an indented outline of tab, group, and page labels, exactly as the sidebar shows them. Read it from the site's navigation config, such as `meta.json` files.

2. **Write eight to twelve tasks.** Base each on something a real reader comes to do. Word each task in the reader's terms, avoiding the label of the page that answers it. Cover every top-level group, add tasks for areas you suspect, and record the correct location for each. More than one location can be correct.

3. **Start a fresh reader.** Use a subagent that starts without this conversation, and give it only the prompt below. Leave out the correct locations.

4. **Score each task.** Record whether the reader reached a correct location, whether its first click was right, and where wrong first clicks landed. A label that draws wrong first clicks from several tasks misleads readers. A task that fails from every path points to content without a findable home.

Done when every task has a score, and each failure names the label or group that caused it.

## Prompt

```text
You are <one line describing the intended reader>.
Below is the navigation of a documentation site. You can see only these labels, not the pages.

For each task, report:
1. The path you would click first, from the top level down.
2. How confident you are, from 1 to 5.
3. Any other path you considered, and why you chose the first.

Tasks:
1. <task>
2. <task>

<navigation>
<indented outline>
</navigation>
```

## Limits

A model reader shows how the labels read to someone outside the project. It does not replace testing with the site's real readers, and it has never been calibrated against them. Run a few tasks with real readers before a large restructure.

## Source

- Nielsen Norman Group, [Tree Testing](https://www.nngroup.com/articles/tree-testing/): a task-based method for checking whether readers can find resources in a category structure and understand its labels.
