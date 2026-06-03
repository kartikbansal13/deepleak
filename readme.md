# DeepLeak: Conversational Strategic Intelligence for AI Race

An automated Open-Source Intelligence (OSINT) data pipeline designed to scrape, translate, summarize, and evaluate deep tech breakthroughs from elite Chinese defense institutions, university research labs, and state publications that are frequently omitted by international mainstream media.

The global race for artificial intelligence and deep tech supremacy is no longer a distant projection—it is a rapidly closing gap. While heavily funded Chinese companies like DeepSeek dominate global headlines when they release a new model, a significant portion of foundational tech breakthroughs happens entirely out of view.
The true starting point for next-generation breakthroughs lies within elite Chinese institutions, state laboratories, and university research hubs. Because these institutions publish their updates almost exclusively in Chinese on localized portals, their progress frequently goes completely unreported by international mainstream media.
For foreign policy experts, defense strategists, and technology analysts, relying solely on mainstream news creates a dangerous blind spot. Academic and institutional research is a leading indicator; what a university lab tests today is what will be deployed in the field three to five years from now. Staying on top of these developments in real time is critical to understanding the future balance of technological power. This automated pipeline bridges that gap by continuously monitoring, translating, and analyzing these hidden channels before they reach the mainstream.

## Architecture 
- **Frontend & Analytics Engine**: Streamlit Framework
- **Automated Compute Infrastructure**: GitHub Actions (Cron Scheduler)
- **LLM Orchestration**: Google Gemini Pro LLM Engine
- **Storage Strategy**: Git-backed Flat-File Versioned Vector Alternative (JSON)

## Implementation Details

The project's automated data pipeline bypasses the need for traditional, expensive cloud infrastructure (like dedicated servers or cloud databases) by creatively using modern developer tools and an optimized AI context window.

## Technical Highlights & Engineering Decisions

*   **Automated Serverless Pipeline:** Uses **GitHub Actions** to run the scraper on a daily schedule. This separates the data collection from the web hosting, meaning the app stays live 24/7 without needing a paid background server.
*   **Git-Backed Data Storage:** Instead of paying for a complex SQL or NoSQL database, the system saves all translated intelligence into a simple **JSON data store** directly in the GitHub repository. The automated bot commits the updates daily, eliminating database maintenance entirely.
*   **In-Context RAG (Retrieval-Augmented Generation):** Rather than setting up an expensive Vector Database, the system leverages the massive 1-million token context window of Gemini 2.5 Flash. The entire JSON database is injected directly into the prompt, allowing the chatbot to answer user questions instantly .
*   **Fault-Tolerant Scraping:** Built with defensive error-handling. If the targeted university websites block the scraper with a firewall, the pipeline catches the error gracefully and automatically loads built-in backup data.
