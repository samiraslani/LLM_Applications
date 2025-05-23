#  AI-Powered Marketing Brochure Generator

**Turn any company website into a beautifully structured marketing brochure in seconds — powered by multi-agent AI intelligence.**

---

##  What It Does

This intelligent system takes a single input — a company URL — and produces a tailored Markdown brochure by automatically:

- Scraping the landing page and internal links using **BeautifulSoup**
- Analyzing which subpages matter most (e.g., *About*, *Services*, *Contact*)
- Summarizing content using both **OpenAI GPT** and **Anthropic Claude** models
- Curating essential information about the company
- Generating a **Markdown-formatted brochure**, ready for investors, customers, or recruitment

It’s like having a **marketing team**, **web crawler**, and **copywriter** in one seamless AI workflow.

---

## Key Strengths

### Multi-Agent Architecture

This system is more than a simple scraper or summarizer. It acts like a **goal-oriented AI agent**:

- **It plans**: Identifies the most useful subpages from a sea of links.
- **It acts**: Visits only the filtered, relevant links.
- **It thinks**: Summarizes information using multiple AI models.
- **It creates**: Generates a clean, concise brochure in Markdown.

Reflects **cutting-edge agentic design**, coordinating multiple steps toward a unified objective.

### Multi-Model Reasoning

Combines the best of both worlds with two leading LLMs:

- **OpenAI GPT-4o** (via `openai`)
- **Anthropic Claude** (via `anthropic`)

This hybrid approach delivers more **accurate**, **insightful**, and **human-sounding** summaries.

---

## Gradio-Powered UI

A sleek and interactive Gradio interface makes the system accessible to all:

1. Paste a company URL
2. Click "Generate"
3. Instantly receive a fully formatted brochure

Run it locally or deploy to the cloud — no coding required.

---

## How It Works

### Step-by-Step Agent Workflow

1. **Website Class**  
   Scrapes body text and collects internal hyperlinks.

2. **Link Filtering Prompt**  
   GPT-4o acts as a filtering agent to identify the most relevant subpages.

3. **Content Extraction**  
   Scrapes and cleans text from selected links.

4. **Prompt Engineering**  
   Custom prompts guide content summarization in a consistent and branded tone.

5. **Brochure Generation**  
   The assistant (OpenAI or Claude) assembles a polished Markdown brochure.

---

## Tech Stack

- **[OpenAI](https://openai.com)** — GPT-4o via Chat Completions API
- **[Anthropic](https://www.anthropic.com/)** — Claude API integration
- **[BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/)** — HTML parsing and scraping
- **[Gradio](https://gradio.app/)** — Browser-based UI framework
- **`dotenv`, `requests`, `json`** — Supporting packages for configuration and stability

---

## Example Output

> Want to see it in action? Run the app, paste a company's website, and watch your custom brochure come to life in seconds.

---

## Contributions & Feedback

Contributions, feature suggestions, and feedback are always welcome! Feel free to open an issue or submit a pull request.

---
## License

MIT License — see `LICENSE.md` for details.
