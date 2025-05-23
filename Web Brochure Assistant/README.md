#  AI-Powered Marketing Brochure Generator

**Turn any company website into a beautifully structured marketing brochure in seconds — powered by multi-agent AI intelligence.**

##  How It Works

This intelligent system transforms a simple user prompt, containing a company name and its URL into a tailored, well-structured **Markdown brochure** using a multi-step agentic workflow:

### End-to-End Process

1. **Prompt Parsing**  
   The system intelligently extracts the company name and website URL from the user’s input prompt.

2. **Website Scraping**  
   Using **BeautifulSoup**, it scrapes the body content of the landing page and all internal hyperlinks.

3. **Link Filtering (via GPT-4o)**  
   A filtering agent determines which internal pages are most relevant (e.g., *About*, *Services*, *Contact*).

4. **Content Extraction & Cleaning**  
   Only the filtered pages are revisited, and their content is re-scraped and cleaned for summarization.

5. **Summarization via LLMs**  
   Content is passed to **OpenAI GPT-4o** or **Anthropic Claude**, depending on user selection, for summarization and branding.

6. **Brochure Generation**  
   The system assembles the curated content into a polished, **Markdown-formatted brochure**. 
---

## Demo 
![Alt text](output.gif)

---

## Key Strengths

### Multi-Agent Architecture

This system is more than a simple scraper or summarizer. It acts like a **goal-oriented AI agent**:

- **It plans**: Identifies the most useful subpages from a sea of links.
- **It acts**: Visits only the filtered, relevant links.
- **It thinks**: Summarizes information using advanced AI models.
- **It creates**: Generates a clean, concise brochure in Markdown.

Reflects **cutting-edge agentic design**, coordinating multiple steps toward a unified objective.

---
### Multi-Model Reasoning

Users can choose between two cutting-edge models to generate the brochure: 

- **OpenAI GPT-4o** (via `openai`)
- **Anthropic Claude** (via `anthropic`)

---

## Gradio-Powered UI

A user-friendly **Gradio interface** provides an intuitive front-end for seamless interaction with the system:

---

## Tech Stack

- **[OpenAI](https://openai.com)** — GPT-4o via Chat Completions API
- **[Anthropic](https://www.anthropic.com/)** — Claude API integration
- **[BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/)** — HTML parsing and scraping
- **[Gradio](https://gradio.app/)** — Browser-based UI framework
- **`dotenv`, `requests`, `json`** — Supporting packages for configuration and stability
---

## Contributions & Feedback

Contributions, feature suggestions, and feedback are always welcome! Feel free to open an issue or submit a pull request.

---
## License

MIT License — see `LICENSE.md` for details.
