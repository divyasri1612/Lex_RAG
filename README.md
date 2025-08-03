# LexRAG: Legal Case Summarization and Retrieval using RAG for New Jersey Tax Court

# 1. Why Did I Start the Project?
I was struggling to file taxes as an international student in March, 2025. No matter how many resources I looked through, it always led to one dead-end, a third party service charging a fortune to file taxes for me. I was tired and wanted to build a smart assistant that could digest massive volumes of dry legal text and produce context-aware summaries and insights for international students struggling to find what is legal and what is not for us. For now, the proving ground is just NJ Tax laws for students on an F1 VISA.

# 3. Main Goal of the Project:
To create a web-based Retrieval-Augmented Generation (RAG) system that scrapes New Jersey Tax Court cases, processes the content, builds embeddings, and answers user queries using retrieved legal precedents. The idea is to assist legal aliens studying/working in the US with quick, relevant legal guidance based on actual case law.

# 4. Work Completed So Far:
Web scraping modules (new.py) to extract year-specific case HTML links.
PDF parsing module (pdf_extractor.py) to extract case content, names, and dates.
Case database and embeddings module (prepping_JSON.py) using SentenceTransformer for semantic search.
Full-stack Flask app (Flask_webpage.py) integrating scraping, vector search, and large language model generation (Flan-T5).
Pytest module (pytest_func.py) with unit tests for scraping, PDF extraction, and metadata parsing.

# 5. Resources Being Used:
Final legal data from law.justia.com
Libraries: PyMuPDF, BeautifulSoup, SentenceTransformers, Transformers, Flask, Scikit-learn, Torch
LLM: Google Flan-T5 Large for response generation

# 6. Timeline:
Scraping pipeline (done)
PDF extraction and metadata parsing (done)
Embedding and vector store setup (done)
Flask app integration and querying UI (done)
Testing, documentation, and final tuning (ongoing)
The base for above mentioned modules has been, it is still a work in progress that needs improvement.

# 7. Future Additions:
Add visual analytics for retrieved case trends.
Expand to other states and court types
Add user query history tracking and personalization.
Fine-tune LLM responses based on feedback from users.
# 8. Tools and Techniques Used:

Web Scraping: Requests, BeautifulSoup, URL parsing
PDF Processing: PyMuPDF for robust extraction
Data Structuring: JSON serialization of case metadata
Vector Embeddings: SentenceTransformer
Semantic Search: Cosine similarity using scikit-learn
Response Generation: HuggingFace Transformers with Flan-T5-Large
Backend: Flask framework for API and web deployment
Testing: Pytest and unittest.mock for modular test coverage
Development Practices: Modular OOP design, CLI-driven debugging, test-first mindset
