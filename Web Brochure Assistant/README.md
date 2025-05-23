#  AI-Powered Marketing Brochure Generator

**Turn any company website into a beautifully structured marketing brochure in seconds — powered by multi-agent AI intelligence.**

---

##  What It Does

This intelligent system takes a two inputs, a company's name and its URL, and produces a tailored Markdown brochure by automatically:

- Scraping the landing page and internal links using **BeautifulSoup**
- Analyzing which subpages matter most (e.g., *About*, *Services*, *Contact*)
- Summarizing content using both **OpenAI GPT** and **Anthropic Claude** models
- Curating essential information about the company
- Generating a **Markdown-formatted brochure**, ready for investors, customers, or recruitment
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

Users can choose between two cutting-edge models to generate the brochure: 

- **OpenAI GPT-4o** (via `openai`)
- **Anthropic Claude** (via `anthropic`)

---

## Gradio-Powered UI

A user-friendly **Gradio interface** provides an intuitive front-end for seamless interaction with the system:

- **Custom Prompt Input**  
  Users can enter a custom prompt that includes the company name and its website URL.

- **Automatic Recognition**  
  The system intelligently parses the prompt to extract the company name and URL.

- **Model Selection**  
  A dropdown menu lets users choose their preferred AI model (e.g., GPT-4o or Claude) for brochure generation.

- **Instant Markdown Output**  
  With a single click, the selected model generates a clean and branded marketing brochure in **Markdown format**.

This browser-based tool is easy to use, requires no programming skills, and can be run locally or deployed to the cloud.

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

## Demo 
![Alt text](images/output.gif)

---

## Contributions & Feedback

Contributions, feature suggestions, and feedback are always welcome! Feel free to open an issue or submit a pull request.

---
## License

MIT License — see `LICENSE.md` for details.
