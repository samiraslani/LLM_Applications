# AI-Powered Website Brochure Generator

Turn any company website into a beautifully crafted brochure — intelligently, efficiently, and automatically.

This system combines multi-agent reasoning, advanced LLM APIs (OpenAI & Anthropic), and a clean Gradio-based interface to build **structured markdown brochures** for companies. It's perfect for marketing, onboarding, investor relations, or recruiting.

---

## ✨ Features

-  **Automated Link Filtering**  
  Smart internal link selection using vector-based semantic relevance.

-  **Multi-Agent LLM Coordination**  
  Combines OpenAI and Anthropic models to generate and refine brochure content through collaborative reasoning.

-  **Multi-Modal Capabilities**  
  Images and visuals are integrated into the brochure for a professional touch.

-  **Live Gradio Frontend**  
  User-friendly interface to preview, edit, and download your brochure.

---

##  Requirements

- Python 3.8+
- OpenAI API key
- Anthropic API key
- Install dependencies:

```bash
pip install -r requirements.txt

---

### OpenAI API Usage

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
## Demo 
<img src="output.gif" width="300"/>


##  Positioning

This tool can serve as:
- A **sales assistant** for agencies building company brochures.
- A **content strategy generator** for marketing teams.
- A **scouting tool** for partnerships and investor research.

---

##  Requirements

- Python 3.8+
- `openai`, `beautifulsoup4`, `requests`, `dotenv`

---

##  Contact

For questions, suggestions, or collaboration ideas, reach out to me at shirinamiraslani@gmail.com.
