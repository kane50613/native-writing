# Documentation

Determine what this document helps the reader do: learn a concept, complete a task, look up a contract, or make a decision. Follow the project's template where it serves that purpose. A readable document can still be detailed and formal.

## Choose the structure by the job

| Document | Useful structure |
| --- | --- |
| README or overview | What this is, who it is for, a working starting point, and routes to deeper material. |
| How-to or help article | Preconditions, actions in order, the expected result, and relevant recovery steps. |
| Conceptual explanation | The idea, a concrete example, how the example works, and where the idea stops applying. |
| API or configuration reference | Exact names, accepted values, defaults, return behavior, errors, and exceptions. |
| Proposal or specification | Problem, proposed behavior, requirements, tradeoffs, and decisions still open. |
| Report or decision record | Finding or decision, supporting evidence, scope, and practical implications. |

Use only the parts the task needs. A how-to should not turn into a history lesson; a design proposal needs enough reasoning for a reviewer to assess it.

## Write for someone who was not in the conversation

Introduce concepts before depending on them. Use consistent terms and explicit references in place of private shorthand. Examples should establish a case, show the operation or reasoning, and show the result. Distinguish sample values from defaults and requirements from suggestions.

Keep prerequisites before the step that needs them, and exceptions near the rule they qualify. Name the relevant version or environment when behavior depends on it. In procedures, use numbered steps when order matters and exact interface labels so readers can find the controls.

Editing prose does not authorize changing commands, signatures, configuration, normative keywords, or promised behavior. Verify technical assertions against the supplied code or authoritative documentation when that is within scope. If the evidence is missing, expose the gap. State whether an example was actually run rather than implying that a plausible snippet was tested.

## Original examples

Brief: workspace owners can invite members through Settings > Members > Invite. The invitation remains pending until accepted. Labels shown here are the product's specified labels.

台灣版：

「只有工作空間擁有者可以邀請成員。

1. 開啟「設定」>「成員」。
2. 點選「邀請」，輸入對方的電子郵件地址。
3. 送出邀請。

對方接受邀請後，才會加入工作空間。」

English version, using the corresponding English UI: “Only workspace owners can invite members. Open Settings > Members, choose Invite, and enter the person's email address. Send the invitation. They join the workspace when they accept it.”

For a short inline answer, this paragraph may suffice. For a help page, separate steps may be easier to follow. Preserve the permission requirement and acceptance condition in both forms.

Specification input: “The export must retain timestamps in UTC. CSV is required for launch. Excel support is under consideration.”

Editing judgment: keep all three statements. The input is already clear; converting “must” to “should,” removing UTC, or implying an Excel commitment would change the specification.

## Completion check

Read as the intended newcomer or reviewer. Check that every needed prerequisite is stated, steps can be followed in order, names match the system, and success or failure is recognizable. Check that a decision document distinguishes evidence, recommendation, and unresolved choices. Preserve the agreed scope and all material exceptions. Use descriptive headings and links to help readers find information again.
