# native-writing

An agent skill for writing and editing app copy, websites, docs, blogs, books, and messages. It adapts wording, tone, and punctuation to the reader and setting while preserving meaning.

Supports [English](references/languages/en/guide.md), [台灣繁中](references/languages/zh-TW/guide.md), and [简体中文](references/languages/zh-CN/guide.md).

## Install

```sh
npx skills add kane50613/native-writing --skill native-writing
```

Add `--global` to make it available across projects.

## Use

Name the audience and where the text will appear:

```text
Use native-writing to edit this README for developers trying the library for the first time.
```

```text
用 native-writing 改寫這個 app 的錯誤提示，給台灣使用者看。
```

## Examples

| Setting | Before | After |
| --- | --- | --- |
| English docs | It is necessary to restart the app in order for the changes to take effect. | Restart the app to apply the changes. |
| 台灣 app | 默認支持上傳視頻，點擊鏈接即可查看文件。 | 預設支援上傳影片，點選連結即可查看檔案。 |
| 简体博客 | 通过引入缓存机制，实现了对重复图片解码操作的有效规避，但缓存失效后仍需重新解码。 | 加上缓存后，同一张图片就不用重复解码。缓存失效后，仍需重新解码。 |

Clear text can stay unchanged. A casual reply like `到了，門口等你` needs no final period. A website notice like `週六暫停服務。週日恢復營業。` keeps its sentence boundaries.

## Add your language

Contribute a language or regional variety you write in, improve an example, or correct local usage. Each language has its own folder under [references/languages/](references/languages/).

See [CONTRIBUTING.md](CONTRIBUTING.md) for the structure, research method, and review process.

[Evaluation cases](evals/README.md) · [MIT License](LICENSE)
