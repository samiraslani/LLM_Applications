# 📄 Web Brochure Assistant using OpenAI GPT

This project creates a **smart assistant** that builds brochures for companies based on the structure and content of their websites. It uses web scraping, prompt engineering, and the OpenAI GPT model to intelligently select which web pages are most useful for a brochure.

---

## 🔍 What It Does

Given a company URL, this system:

1. Scrapes the main content and all subpage links using `BeautifulSoup`.
2. Crafts a **system prompt** and a **user prompt** with structured instructions.
3. Calls the **OpenAI API** with those prompts to:
   - Understand the site context.
   - Choose only the most relevant subpages (e.g., About, Services, Contact).
4. Optionally gathers content from the selected links.
5. Constructs a brochure prompt or markdown-ready summary using the filtered information.

---

## Key Concepts

### Agentic Thinking

This architecture mirrors the **agentic workflow**:
- The assistant receives context (`Website` class).
- It makes decisions (`link filtering`).
- It takes actions (`fetch content`, `build brochure`).
This is similar to how **AI agents** plan and act across multiple steps.

### OpenAI API Usage

The system sends **multi-turn chat messages** to GPT:
- `system_prompt`: Sets behavior (e.g., "You are a helpful assistant for filtering links").
- `user_prompt`: Gives specific input (e.g., site links and goal).
This results in multiple API calls when:
- The site is parsed.
- Content for each subpage is gathered.
- Final brochure summary is generated.

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
