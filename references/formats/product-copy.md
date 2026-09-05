# Website and app copy

Start from the surface and the behavior. Read the brief, existing screens or strings, and relevant implementation when available. Identify what the person knows here, what they need to decide, and what each action actually does. If a material behavior is unspecified, ask or mark it as an open product question rather than make up a promise.

## Marketing pages

Give the intended customer a reason to care, using a concrete capability, outcome, or situation supported by the product. A headline can be expressive; nearby copy should make its meaning clear. Match the CTA to its destination: requesting a demo, creating an account, and starting a paid subscription are different actions.

Choose sections around the visitor's questions. Explain who the product serves, what it helps them do, and the evidence or conditions they need to decide. Benefits can be persuasive without invented statistics, customer quotes, superiority claims, or implied features. Put material trial, price, and renewal conditions near the relevant decision using the supplied terms.

Original example brief: restaurants can send customers a link to check their queue position without installing an app. The CTA opens a demo request form.

- 台灣：標題「候位進度，手機就能看」。說明「把候位連結傳給客人，打開就能查看排到哪裡，不用下載 app。」按鈕「預約展示」。
- 简中：标题“在手机上查看排队进度”。说明“把排队链接发给顾客，打开就能查看进度，无需下载 App。”按钮“预约演示”。
- English: “Check your place in line from your phone.” Supporting copy: “Send guests a link to check their place in line without installing an app.” CTA: “Request a demo.”

These are three versions of one brief, not literal translations of a slogan. The benefit belongs to guests while the purchase decision belongs to restaurants; preserve that distinction.

## Interface text

Use familiar, stable names for objects and actions. A button can be a short label; it does not need to be a conversational sentence. Read it alongside its heading and helper text so the parts work together without repeating everything.

| Surface | What the text must resolve |
| --- | --- |
| Button or link | What happens when this is activated? Name the action and object where needed. |
| Field | What belongs here? Put format or eligibility help where it is needed; keep a persistent label. |
| Empty state | Is this new, filtered to no results, or unavailable? Offer the next action that exists for that state. |
| Progress | What is happening now? Use a time estimate only when the product can support it. |
| Error | What failed, what is known about the cause, and what can this person do next? |
| Success | What completed? Distinguish sending, receiving, processing, and approval. |
| Destructive confirmation | What object is affected, what is lost, and whether it can be recovered? Name the destructive action. |

Make recovery text actionable and accurate. A network error is not proof that data was lost, and an unconfirmed payment is not proof that no charge occurred. Tell the person what the product knows; avoid inventing a cause or suggesting a retry that might duplicate an action. Keep debugging internals out unless the intended user needs them.

Original examples:

- No projects yet, with project creation available: 「還沒有專案」／「建立第一個專案」.
- A filter matches no existing projects, with reset available: 「沒有符合條件的專案」／「清除篩選」.
- Deletion is permanent and includes all files. Title: 刪除「春季活動」？ Body: 專案內的所有檔案都會一併刪除，刪除後無法復原。 Buttons: 保留專案 / 刪除專案.
- File upload succeeds but processing continues: “Upload complete. We're processing your file.” This is not yet a message that the file is ready to use.

## Completion check

Walk through the strings in screen order, including the relevant alternate states. Each action must match the behavior; each condition must appear before it matters. Verify names, variables, plural forms, units, and links against the product. Preserve interpolation tokens and translation keys when editing a catalog. Check actual layout when available, especially narrow screens and longer translations; otherwise describe fit as unverified. Do not remove a necessary word merely to match another language's character count.

Return copy grouped by its screen or component, or edit the requested files. Keep implementation notes separate from customer-facing text.
