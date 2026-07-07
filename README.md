# Atrail AI for Excel

> **Beta Software** — This is an early release. Features may change, bugs may exist. Always keep a backup of important workbooks before using AI to modify them.

An AI assistant built into Excel. Ask it to sort, clean, analyse, build pivot tables, add formulas, and more — all in plain English.

Supports **Anthropic Claude · OpenAI GPT · DeepSeek · xAI Grok · Gemini · OpenRouter**

---

## Requirements

- Windows 10 or 11
- Excel 2016 or later (64-bit recommended)
- An API key from at least one AI provider

No additional software needs to be installed. The .NET runtime is bundled inside the add-in.

---

## Installation

1. Download **Atrail Excel Addin.xll** from this page
2. Open Excel
3. Go to **File > Options > Add-ins**
4. At the bottom, set "Manage" to **Excel Add-ins** and click **Go**
5. Click **Browse**, select the `.xll` file, click **OK**
6. Tick the checkbox next to **Atrail AI**, click **OK**
7. The Atrail panel opens on the right side of Excel

> To reopen the panel later: **Add-ins tab > Atrail AI**

---

## Getting an API Key

You need a key from at least one provider. All offer free tiers or trial credits.

| Provider | Sign up | Notes |
|---|---|---|
| **Anthropic** | console.anthropic.com | Best reasoning. Claude models. |
| **OpenAI** | platform.openai.com | GPT-4o, o4-mini, o3. |
| **DeepSeek** | platform.deepseek.com | Very low cost. Includes reasoning model. |
| **xAI / Grok** | console.x.ai | Grok 3 models. |
| **Gemini** | aistudio.google.com | Free tier available. |
| **OpenRouter** | openrouter.ai | Access many models with one key. |

Once you have a key: click **... > Settings** in the panel, paste the key, choose your provider and model, click **Save**.

---

## Using Atrail AI

Type your request in the chat box and press **Enter**.

**Example requests:**
- "Sort this table by revenue, highest first"
- "Add a total row at the bottom"
- "Highlight all cells below 100 in red"
- "Create a pivot table showing sales by region"
- "Remove duplicates based on column A"
- "Add a Yes / No / Pending dropdown to column D"
- "Write a formula that calculates the 3-month rolling average"

### Scope
The toolbar shows the current scope — click it to cycle between **Sheet**, **Selection**, and **Workbook**.

### Permissions
For destructive actions (deleting rows, clearing data) the AI asks for your approval first. Click **Accept All Edits** to skip prompts for the current session.

---

## Privacy

Your spreadsheet data is sent to the AI provider you selected to process your request. Atrail itself never sees or stores it.

Your API key is encrypted using Windows built-in security (DPAPI) and stored only on your computer, tied to your Windows user account. It is never sent to Atrail, never written to a plain text file, and is masked on screen so it cannot be seen by others. Atrail has no server, no account system, and no usage tracking of any kind.

Review your chosen provider's privacy policy before using confidential data.

---

## Updates

The add-in checks for updates every 30 days. A green banner appears when a new version is available — click it to download. To check immediately: **... > Check for updates**.

To update: download the new `.xll` and repeat the installation steps (Excel will ask you to replace the old one).

---

## Troubleshooting

**Add-in did not load** — Make sure you are using 64-bit Excel on Windows 10 or 11.

**"No API key" warning** — Open **... > Settings** and add your key.

**HTTP 401 error** — Your key is invalid or expired. Check it in your provider's dashboard.

**Panel does not open** — Go to the **Add-ins** tab in Excel's ribbon and click **Atrail AI**.

---

## Support

GitHub: https://github.com/officialatrail/Atrail-Excel-Addin

---

## Disclaimer

Atrail AI is beta software, provided as is. It works well for most tasks but is still in testing and may not always give perfect results. Please review any changes the AI makes to your spreadsheet before relying on them.

- **AI output:** The AI is powered by third-party models. Atrail cannot guarantee that every formula, edit, or suggestion will be correct. Always check the results.
- **Your data goes to your AI provider:** When you ask a question, the relevant parts of your spreadsheet are sent to the AI provider you configured. By using this add-in you agree to that provider's own terms and privacy policy. Atrail has no control over how they handle your data.
- **API costs:** Any charges from your AI provider are billed directly to you. Atrail does not charge for the add-in and is not responsible for third-party billing.
- **No affiliation:** Atrail AI is an independent product, not made by or affiliated with Microsoft Corporation.
- **Liability:** To the extent allowed by law, Atrail accepts no liability for data loss, errors in AI output, or any other damage arising from use of this software.
