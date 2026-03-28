# Getting Started with Claude for Finance & Business

> Your guide to using Claude as a financial analysis tool — not just a chatbot.

---

## What You Need to Know First

Claude isn't just for writing essays. Major financial institutions — Visa, Citigroup, Bridgewater, Moody's, RBC Capital Markets — are already using it for real financial analysis. In benchmarks, Claude outperforms Microsoft Copilot on financial tasks like income statement forecasting and data sourcing.

You have a **Pro account** and access to **Claude Code**. That gives you serious capabilities.

---

## Part 1: The Claude App (claude.ai)

### What You Can Upload

You can drag and drop files directly into Claude and ask questions about them:

| File Type | Example |
|-----------|---------|
| **Excel (.xlsx)** | A budget spreadsheet, financial model, or dataset |
| **CSV** | Stock price data, transaction records, any tabular data |
| **PDF** | Annual reports, earnings reports, company filings |
| **Word (.docx)** | Research reports, investment memos |

### Try This Right Now

1. Go to `claude.ai`
2. Download any public annual report (Google "Apple annual report 2025 PDF" or "Tesco annual report 2025 PDF")
3. Upload it and type:

> You are a senior equity analyst at Goldman Sachs. Analyse this annual report. Cover: revenue growth trends, profit margin changes, balance sheet health, key risks, and your overall investment thesis. Present findings in a structured format.

4. Read the output. Then ask follow-up questions:
   - "How would a recession affect this company?"
   - "Compare the debt levels to industry average"
   - "Explain the P/E ratio in simple terms"

The follow-up conversation is where the real learning happens.

---

### Anthropic's Official Prompts

Anthropic maintains a prompt library with pre-built prompts you can use. Two are directly useful:

**Corporate Clairvoyant** (from Anthropic's original prompt library)
- Designed specifically for analysing company reports
- Covers growth, profitability, balance sheet health, and business momentum
- Try this system prompt: *"You are a corporate analyst. Analyse this report covering top-line growth, profitability, balance sheet health, and business momentum. Identify key risks and opportunities."*

**Excel Formula Expert** (from Anthropic's original prompt library)
- Describe what you want a formula to do in plain English
- Claude writes the formula and explains how it works
- Try this system prompt: *"You are an Excel expert. I'll describe what I want a formula to do, and you'll write the formula and explain how it works step by step."*

For general prompting tips, visit `platform.claude.com/docs/en/resources/prompt-library/library`

---

### The "Role Prompting" Technique

This is the single most important thing to learn. Compare these two approaches:

**Without role prompting:**
> Analyse Apple's revenue

**With role prompting:**
> You are a senior equity analyst at Morgan Stanley who has covered Apple for 10 years. Analyse Apple's revenue trajectory over the last 3 years, including segment breakdown, growth drivers, and risks to forward estimates. Format as an analyst note.

The second prompt will give you something that looks like a real analyst report. The first will give you a generic summary. **Always tell Claude who it should be.**

---

### Tips That Actually Matter

1. **Put the document first, question second** — Claude analyses better when it reads the data before seeing your question (Anthropic says this improves quality by ~30%)
2. **Be specific** — "Analyse revenue growth over the last 3 years and identify the main driver" beats "Tell me about this company"
3. **Ask for specific formats** — "Present as a table", "Format as bullet points", "Write as a one-page memo"
4. **Iterate** — the first answer is a starting point. Push back, ask for more detail, challenge assumptions
5. **Specify UK context** — Claude defaults to US financial systems. Add "Use UK tax rates and financial regulations" when relevant

---

## Part 2: Claude Code (Terminal)

Claude Code lets you go beyond uploading files — you can build things.

### What Claude Code Can Do That the App Can't

- Read and analyse files directly from your computer without uploading
- Write scripts that process multiple files at once
- Build simple web pages and dashboards
- Connect to free financial data APIs
- Automate repetitive analysis tasks

### Starter Projects

Pick one that interests you and build it with Claude Code:

**Beginner: CSV Spending Analyser**
- Create a CSV of monthly expenses (or use a sample one)
- Ask Claude Code to read it and generate a summary: total spending, biggest categories, trends
- Output as a clean markdown report

**Beginner: Excel Formula Builder**
- Describe a financial calculation you need
- Have Claude Code create the Excel formula and explain every part
- Test it in a real spreadsheet

**Intermediate: Stock Data Fetcher**
- Use a free API (like Alpha Vantage — free key available) to pull stock price data
- Claude Code writes the script, you run it
- Extend it: add comparisons between two stocks, calculate basic metrics

**Intermediate: Personal Budget Dashboard**
- Build a simple HTML page that reads a CSV of your expenses
- Shows charts, totals by category, month-over-month comparison
- Deploy it for free on Vercel

**Advanced: Earnings Report Summariser**
- Download a company's earnings report PDF
- Have Claude Code write a script that extracts key metrics
- Generate a one-page summary automatically

---

## Part 3: What the Professionals Use

You can't access these features on a Pro plan, but knowing they exist is important for understanding where finance + AI is heading.

### Enterprise Financial Skills (Built into Claude)

| Skill | What It Does |
|-------|-------------|
| Comparable company analysis | Builds valuation tables comparing similar companies |
| Discounted cash flow model | Creates full DCF models with sensitivity analysis |
| Due diligence data pack | Converts raw filings into structured spreadsheets |
| Earnings research | Automatically extracts key metrics from earnings calls |
| Initiating coverage report | Produces full investment research reports |

### Live Data Connections

Enterprise Claude connects directly to:
- **LSEG** — live market prices (equities, FX, bonds, macro data)
- **Moody's** — credit ratings on 600+ million companies
- **Aiera** — earnings call transcripts
- **MT Newswires** — real-time financial news

### Claude Inside Excel

Claude now works as a sidebar inside Microsoft Excel (Teams/Enterprise). It can:
- Explain how a spreadsheet works
- Modify formulas while keeping everything else intact
- Debug cell errors
- Build a financial model from scratch

People have documented building complete 11-tab financial models in under 10 minutes.

---

## Part 4: Important Limitations

Be honest about what Claude can't do:

| Limitation | Why It Matters |
|------------|---------------|
| **Not investment advice** | Claude analyses — it doesn't know your personal circumstances or risk tolerance |
| **Can make arithmetic errors** | Always verify calculations, especially in Excel formulas |
| **No real-time data** (on Pro) | It can't check today's stock price — you'd need to provide the data |
| **Can hallucinate data** | It may invent plausible-sounding numbers. Cross-reference everything |
| **US-centric defaults** | Specify "UK context" when discussing tax, pensions, ISAs, student loans |

**The golden rule**: Use Claude to accelerate your thinking, not replace it. A financial analyst uses Claude to do in 10 minutes what used to take 2 hours — but they still check the work.

---

## Videos Worth Watching

These are from Anthropic (the company that makes Claude). Browse all at `anthropic.com/events`:

- **How to Transform Work with Claude for Excel and PowerPoint** — `anthropic.com/webinars/claude-in-excel-and-powerpoint`
- **Advancing Claude for Financial Services** — `anthropic.com/webinars/claude-for-financial-services`
- **How BCI Leverages Claude's Financial Analysis** — `anthropic.com/webinars/bci-claude-financial-analysis`

---

## What to Try This Session

1. **Upload a real annual report** to claude.ai and use the role prompting technique
2. **Try one of the prompts** from the [sample-scenarios.md](sample-scenarios.md) file — pick a character, pick a prompt, see what Claude produces
3. **Ask follow-up questions** — don't just accept the first answer. Challenge it, ask for simpler explanations, change the numbers
4. **If you're comfortable**: Open Claude Code and try reading a CSV file directly from the terminal

---

## Useful Links

| What | Where |
|------|-------|
| Claude app | `claude.ai` |
| Prompting best practices | `platform.claude.com/docs/en/resources/prompt-library/library` |
| Financial services overview | `claude.com/solutions/financial-services` |
| Financial services tutorial | `claude.com/resources/tutorials/claude-for-financial-services-overview` |
| Events & webinars | `anthropic.com/events` |
| Excel & PowerPoint webinar | `anthropic.com/webinars/claude-in-excel-and-powerpoint` |
| Economics AI tools | `meleantonio.github.io/awesome-econ-ai-stuff/` |

---

> **Remember**: The students who learn to work effectively with AI tools now will have a genuine advantage when they enter the workplace. This isn't about replacing human thinking — it's about having a tool that lets you think faster and deeper.
