# Atrail AI for Excel

An AI assistant built directly into Excel. Ask it to sort, clean, analyse, build pivot tables, add formulas, and more — all in plain English.

Supports **Anthropic Claude · OpenAI GPT · DeepSeek · xAI Grok · Gemini · OpenRouter**

---

## Requirements

- Windows 10 or 11
- Excel 2016 or later (64-bit)
- [.NET 10 Desktop Runtime](https://dotnet.microsoft.com/en-us/download/dotnet/10.0) — free, one-time install from Microsoft (~25 MB)

---

## Installation

1. Install [.NET 10 Desktop Runtime](https://dotnet.microsoft.com/en-us/download/dotnet/10.0) if you have not already
2. Download **Atrail Excel Addin.xll** from this page
3. Open Excel → **File → Options → Add-ins**
4. Set "Manage" to **Excel Add-ins** and click **Go**
5. Click **Browse**, select the `.xll` file, click **OK**
6. Tick the checkbox next to **Atrail AI** and click **OK**

> To reopen the panel later: **Add-ins tab → Atrail AI**

---

## Getting Started

You need an API key from at least one provider, or sign in with OpenRouter for instant access.

### Option A — OpenRouter (easiest, free models available)

OpenRouter lets you access many AI models with one login — no API key to copy and paste.

1. Click **⋯ → Settings** in the panel
2. Scroll to **OpenRouter** and click **Connect with OpenRouter**
3. Approve in your browser — done

Free models (no credits needed): Llama 4, Qwen 3, DeepSeek R1, Gemini Flash, and more.  
Paid models: Claude, GPT-4, Gemini Pro, Grok — charged to your OpenRouter balance.

### Option B — Direct API key

| Provider | Sign up | Notes |
|---|---|---|
| **Anthropic** | console.anthropic.com | Claude models. Best reasoning. |
| **OpenAI** | platform.openai.com | GPT-4.1, o3, o4-mini. |
| **DeepSeek** | platform.deepseek.com | Very low cost. R1 reasoning model. |
| **xAI / Grok** | console.x.ai | Grok 3. |
| **Gemini** | aistudio.google.com | Free tier available. |

Paste the key in **⋯ → Settings**, choose your provider and model, click **Save**.

---

## What You Can Do

Type your request in the chat box and press **Enter** (or the arrow button).

**Examples:**
- "Sort this table by revenue, highest first"
- "Add a total row at the bottom"
- "Highlight all cells below 100 in red"
- "Create a pivot table showing sales by region"
- "Remove duplicates based on column A"
- "Add a Yes / No / Pending dropdown to column D"
- "Write a VLOOKUP formula to match order IDs"
- "Summarise what's in this sheet"

### Scope
The toolbar shows the current scope. Click it to cycle:
- **Sheet** — reads and edits the active sheet
- **Selection** — works only on the selected range
- **Workbook** — sees all sheets

### Sheet Lock
Pin the AI to a specific sheet with the **○** button next to the sheet name. Even when you navigate to other sheets, the AI will continue reading from and writing to the locked sheet.

### Thinking Mode
Toggle extended reasoning with the **≈** button. Useful for complex formulas and analysis.

### Permissions
For destructive actions (deleting rows, clearing data) the AI asks for approval first. Click **Accept All** to skip prompts for the session.

---

## Privacy

Your spreadsheet data is sent to the AI provider you chose to process your request. It is not stored by Atrail. Review your provider's privacy policy before using confidential data.

API keys are encrypted on your machine using Windows DPAPI and never leave it.

---

## Updates

The add-in checks for updates automatically. A banner appears when a new version is available — click it to download. To check manually: **⋯ → Check for updates**.

To update: download the new `.xll`, open Excel Add-ins, and browse to replace the old file.

---

## Troubleshooting

**Add-in did not load** — Install [.NET 10 Desktop Runtime](https://dotnet.microsoft.com/en-us/download/dotnet/10.0) and restart Excel.

**"No API key" message** — Open **⋯ → Settings** and add your key or connect OpenRouter.

**HTTP 401 error** — Your key is invalid or expired. Disconnect and reconnect OpenRouter, or check the key in your provider's dashboard.

**Panel does not open** — Go to the **Add-ins** tab in Excel's ribbon and click **Atrail AI**.

**White or invisible text** — Open **⋯ → Settings**, switch Theme to Dark, save, then switch back.

---

## Support

Website: https://officialatrail.online  
GitHub: https://github.com/officialatrail/Atrail-Excel-Addin
