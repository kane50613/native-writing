# Behavioral review

These are manual evaluation cases, not an automated benchmark or a record of passing results. Run each prompt in a fresh agent context with the skill available. Save the exact prompt and output with the model, date, and skill revision when reporting results.

Judge whether the result communicates the intended meaning in the requested language and form. Wording may vary. A factual invention, lost condition, or changed commitment is a failure even if the prose sounds smooth.

## Cases

| Case | Prompt | Review criteria |
| --- | --- | --- |
| Evidence limits | Use native-writing to edit: “The cache delivered a significant performance enhancement, reducing startup from 800 ms to 500 ms in one local test, although its production impact has yet to be validated.” | Keeps both numbers, the single local test, and the lack of production validation. |
| Already clear | Use native-writing to edit: “The preview updates immediately, but saving still takes about two seconds.” | Preserves the contrast and approximate duration. Leaving it unchanged is appropriate. |
| Taiwan product copy | 用 native-writing 寫台灣 app 的上傳錯誤提示。已確認檔案超過 10 MB，使用者可以重新選擇檔案。需要標題、說明、按鈕。 | Uses Taiwan terminology, states the size limit accurately, and offers the available action. No invented file-type restriction or retry behavior. |
| Mainland product copy | 用 native-writing 写简体中文的上传错误提示，面向中国大陆用户。已确认文件超过 10 MB，用户可以重新选择文件。需要标题、说明、按钮。 | Uses natural mainland terminology and the same known conditions. Does not import Taiwan vocabulary mechanically. |
| Literal labels | 用 native-writing 改成台灣繁中，保留外部工具的實際按鈕名稱：點擊「保存文件」即可把文件保存到你的電腦。 | Preserves the quoted label exactly while adapting surrounding prose to Taiwan usage. |
| Uncertain payment | Use native-writing to write an English payment error. The request timed out. We do not know whether a charge occurred. The user can check payment status on the Orders page. | Gives the known next step. Does not promise no charge or encourage an immediate repeat payment. |
| Documentation | Use native-writing to edit: “Only workspace owners can invite members. Invitations stay pending until accepted. All timestamps must be UTC.” | Retains owner-only permission, the acceptance condition, and the mandatory UTC requirement. |
| Blog voice | 用 native-writing 修改：我之前一直觉得搭博客很麻烦。周末试了一下，发现最费时间的其实是挑主题，文章反而一篇没写。 | Preserves the sequence and self-deprecating observation. Does not fabricate an anecdote or add a moral. Leaving it unchanged is appropriate. |
| Code punctuation | Use native-writing to edit this sentence, keeping the code exact: Run `SELECT 1;` to check the connection. | Leaves the SQL semicolon and command unchanged. |
| Missing substance | 用 native-writing 改寫對外公告：這次更新大幅提升了效能，為使用者帶來前所未有的流暢體驗。 | Adds no measurements or features. Briefly flags missing evidence when needed for the public claim. |

For a new language, include everyday prose, a product string, a developed explanation, and an already-clear passage. A fluent reviewer familiar with the target region should assess naturalness. Keep those judgments separate from mechanically checkable facts.

## Punctuation by language

- [English](en.md)
- [台灣繁中](zh-TW.md)
- [简体中文](zh-CN.md)

These fixtures cover message endings, developed prose, fiction, UI strings, and literal syntax. They have not yet been run as a controlled model comparison.
