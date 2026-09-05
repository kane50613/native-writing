# native-writing

An agent skill for writing website and app copy, docs, blogs, and messages in natural language.

Supports [English](references/languages/en/guide.md), [台灣繁中](references/languages/zh-TW/guide.md), and [简体中文](references/languages/zh-CN/guide.md), with guidance on local vocabulary, tone, and sentence structure.

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

## Examples

Original editing examples:

| | Before | After |
| --- | --- | --- |
| English · docs | The implementation introduces a retry-boundary ownership model: the caller decides whether a failed request should be retried. | The caller decides whether to retry a failed request. |
| 台灣繁中 · app | 默認支持上傳視頻，點擊鏈接即可查看文件。 | 預設支援上傳影片，點選連結即可查看檔案。 |
| 简体中文 · blog | 通过引入缓存机制，实现了对重复图片解码操作的有效规避，但缓存失效后仍需重新解码。 | 加上缓存后，同一张图片就不用重复解码。缓存失效后，仍需重新解码。 |

## Contribute your language

Help us add the languages and regional varieties you write in. Contribute writing guidance, before-and-after examples, or corrections backed by local usage.

Start in [`references/languages/`](references/languages/). Each language has its own folder. See [CONTRIBUTING.md](CONTRIBUTING.md) for what to include and where it belongs.

[Research](references/research/initial-samples.md) · [Evaluation cases](evals/README.md) · [MIT License](LICENSE)
