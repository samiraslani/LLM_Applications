# 📄 Web Brochure Assistant using OpenAI GPT

This project builds a **smart assistant** that generates professional brochures for companies based on the structure and content of their websites. It combines **web scraping**, **prompt engineering**, and the **OpenAI GPT model** to intelligently select the most relevant web pages for brochure content.

---

## 🔍 What It Does

Given a company URL, the system:

1. Scrapes the main content and subpage links using `BeautifulSoup`.
2. Constructs structured prompts:
   - **System prompt**: Sets the assistant's behavior.
   - **User prompt**: Supplies specific task instructions and content.
3. Uses the **OpenAI GPT API** to:
   - Understand the site's context.
   - Select only the most relevant subpages (e.g., About, Services, Contact).
4. Optionally fetches and processes content from the selected subpages.
5. Generates a **markdown brochure** using the curated content.

---

## 🧠 Key Concepts

### Agentic Thinking

The architecture mirrors an **agent-like workflow**:

- The assistant receives context using a `Website` class.
- It extracts and evaluates all internal links from the main website.
- It **decides** which links are useful for brochure generation (link filtering).
- It takes **actions** by fetching and summarizing content from those relevant links.
- It **generates** a final brochure based on the gathered information.

This mimics how **AI agents** plan and act in multiple steps toward a goal.

---

### 🤖 OpenAI API Usage

The system communicates with GPT using **multi-turn chat messages**:

- `system_prompt`: Defines behavior (e.g., *“You are a helpful assistant for filtering links”*).
- `user_prompt`: Provides detailed input (e.g., list of links, desired brochure format).

This results in **multiple API calls** during:

- Link filtering phase (deciding which pages matter).
- Brochure generation phase (writing the actual content in markdown).

You can choose between:
- **One-shot prompting**: Pass all context in one go (fast, concise).
- **Few-shot prompting**: Provide multiple examples for richer understanding (more robust).

---

## How to Use

1. Clone this repo and add your OpenAI API key to a `.env` file:
    ```env
    OPENAI_API_KEY=your_key_here
    ```

2. Run the notebook:
    ```python
    from openai import OpenAI
    from Website import Website

    get_brochure_user_prompt("BBC", "https://www.bbc.com")
    ```

3. Modify the prompt, model (e.g., `gpt-4o`), or link parser as needed.


---

## 💼 Positioning

This tool can serve as:
- A **sales assistant** for agencies building company brochures.
- A **content strategy generator** for marketing teams.
- A **scouting tool** for partnerships and investor research.
- A **knowledge organizer** for product managers.

---

## 👨‍💻 Requirements

- Python 3.8+
- `openai`, `beautifulsoup4`, `requests`, `dotenv`

---

## 📣 Contact

For questions, suggestions, or collaboration ideas, reach out to me at shirinamiraslani@gmail.com.
