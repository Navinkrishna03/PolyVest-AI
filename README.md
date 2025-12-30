PolyVest: Your AI Funding Companion
PolyVest is a multilingual, RAG-based AI agent designed to democratize access to startup funding knowledge for Indian founders. It bridges the gap between complex financial policies and vernacular understanding, cross-referencing official government schemes with real-time market data.

Key Features :
Multilingual Support (Bharat-First):
Native support for Hindi, Tamil, and English.
Simplifies complex financial terms (e.g., "Equity Dilution," "Term Sheets") into local metaphors.

Live Pitch Deck Analyst:
Upload pitch decks (PDF/TXT).
Generates a structured "Funding Readiness Scorecard" (0-10).
Checks eligibility against government schemes (e.g., SISFS).

Cross-Referencing Engine:
Validates user asks against official policy limits and current market valuations.
Detects "Red Flags" like missing revenue models or ineligible age criteria.

Professional Reporting:
Generates downloadable Funding Reports in PDF and PPT formats.

Privacy-First:
Uses local embeddings (HuggingFace) to ensure sensitive pitch data never leaves the session.
Auto-wipes uploaded files upon session refresh.

Tech Stack :
Frontend: Streamlit
LLM: Llama 3.3 (via Groq API)

Orchestration: LlamaIndex

Embeddings: HuggingFace (sentence-transformers/all-MiniLM-L6-v2)

Document Generation: FPDF (PDF), python-pptx (PowerPoint)

Setup & Usage
Clone Repository: git clone [repository-url] cd PolyVest

Install Dependencies: pip install -r requirements.txt

Configure API Key:
Create a .streamlit/secrets.toml file.
Add: GROQ_API_KEY = "your_key_here"

Run Application: streamlit run app.py

Usage:
Ask questions about funding schemes in your preferred language.
Upload a pitch deck to receive a comprehensive analysis and download reports.

License :
This project is open-source under the MIT License.
