# Slides and presentation decks

First decide whether a speaker presents the deck or the audience reads it alone. A presented slide can leave the explanation to the speaker. A deck sent ahead, or handed in as a report, must carry its own explanation, so each slide needs a little more text. Ask when the request leaves this open and the answer changes how much each slide says.

## Headline states the point

Write each headline as the sentence the slide proves, not a topic label. "Revenue streams" becomes "The code is free, and companies pay for support". The body holds the evidence for that sentence: a chart, an image, a diagram, or a few short lines. In one controlled comparison, students who saw sentence headlines over visual evidence understood and recalled more than students who saw topic headlines over bullets.

Keep a headline to one or two lines at the size the slide is shown. Break it at a phrase boundary. In Chinese and Japanese, renderers can break inside a word, so set the break by hand when the headline wraps.

## One point, three items

Give each slide one point. Support it with at most three items, and merge, cut, or move the rest to another slide or the speaker's notes. Three is about what an audience keeps from a short talk without taking notes.

## Lines the audience can read from the back

Write items as phrases or short sentences that each fit on one or two lines. Body text has to stay large enough to read from the back of the room, which limits how many words a slide can hold. For a meeting room, one Taiwanese type guide puts body text at 24 pt or larger, with headlines 1.5 to 2 times the body size.

Name each advantage by what changes for this audience. For an audience outside the field, replace jargon with an everyday comparison, and keep the technical term only where the audience will use it. A comparative claim such as "faster" or "cheaper" needs a measurement from the input. Show the number on the slide with its conditions in a footnote, or flag the gap.

End slide lines the way the language guide's punctuation reference says for slides.

## Original example

Brief: explain to a teacher outside computing why companies would pay for Takumi, a library that turns web designs into images and PDFs. A benchmark rendered the same two-page invoice 20 times on an M1 Pro. The median was 26 ms for Takumi and 201 ms for Puppeteer with Chrome.

Before:

> 價值主張
>
> - 不需 headless browser，一套排版輸出 PNG、GIF、PDF、SVG
> - 比 Puppeteer 類方案更快、更省運算成本
> - 可在 Edge 與 Serverless 執行
> - 沿用 JSX、HTML、Tailwind

After:

> 不必開瀏覽器，產生 PDF 快將近 8 倍
>
> （長條圖：Takumi 26 ms，Puppeteer + Chrome 201 ms）
>
> 現在的做法，像是為了印一張名片，先開一整間印刷廠
>
> 註：同一份兩頁發票，在 M1 Pro 筆電上各產生 20 次取中位數

The headline turns the topic into the claim, and the chart carries its evidence. "8 倍" comes from the supplied benchmark, and the footnote keeps its conditions. The comparison replaces "headless browser" for a reader who has never run one. Edge and Serverless leave the slide because they do not support this headline.

## Completion check

Read only the headlines, in order. Together they should tell the whole argument. On each slide, check that every item supports the headline and that no slide has more than three items. Every number shows its source or conditions. Every term is one this audience already uses, or the slide explains it. When a rendered deck is available, check that each line fits and no single character wraps onto a line of its own.

## Sources

- Joanna K. Garner and Michael P. Alley, [“How the design of presentation slides affects audience comprehension: A case for the assertion-evidence approach”](https://pure.psu.edu/en/publications/how-the-design-of-presentation-slides-affects-audience-comprehens/), *International Journal of Engineering Education* 29(6), 2013. One experiment with 110 engineering students. Penn State keeps a [summary of the related research](https://writing.engr.psu.edu/research.html).
- 謝文憲 and 王永福, 《千萬講師的50堂說話課》 (Business Weekly Publications), [excerpted by 104](https://blog.104.com.tw/less-is-more-presentation/): a ten-minute talk covers three points, because that is what listeners remember without notes.
- National Taiwan University Library, [slide design handout](https://www.lib.ntu.edu.tw/img/tulblog/HELP/HELP_20230420_Slidetips.pdf) (2023), citing 王永福's 《上台的技術》: one point per slide.
- justfont, [“簡報文字易讀性”](https://blog.justfont.com/2023/12/slide-readability/) (2023): body text of at least 24 pt for meeting-room projection, and headlines 1.5 to 2 times the body size.
- ManyPixels, [“The complete guide to pitch deck design in 2026”](https://www.manypixels.co/blog/presentations/pitch-deck-design): a deck read alone and a deck presented live need different amounts of text.
