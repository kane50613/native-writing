# native-writing

An agent skill for writing website and app copy, docs, blogs, and messages in natural language.

Supports [English](references/english.md), [台灣繁中](references/zh-tw.md), and [简体中文](references/zh-cn.md), with guidance on local vocabulary, tone, and sentence structure. More languages are welcome.

## Install

```sh
npx skills add kane50613/native-writing --skill native-writing
```

Add `--global` to install across projects.

## Use

Ask your agent to use `native-writing` and describe the audience:

```text
Use native-writing to edit this README for developers new to the library.
```

```text
用 native-writing 改寫這個 app 的錯誤訊息，給台灣使用者看。
```

One skill, with references loaded by language and writing format. Based on samples from communities, blogs, documentation, and product pages.

[Research](references/community-research.md) · [Contributing](CONTRIBUTING.md) · [Evaluation cases](evals/README.md) · [MIT License](LICENSE)
