# 📄 AI-Driven Resume Parser Engine

An intelligent, modular parsing engine built in Python that automatically extracts, segments, and transforms unstructured resume PDFs into highly structured, clean JSON artifacts. This tool bridges the gap between raw document extraction and automated Applicant Tracking Systems (ATS).

## 🚀 Overview

This project employs a hybrid data-extraction methodology combining **deterministic rule-based heuristics** with **statistical Natural Language Processing (NLP)** to achieve high precision and recall across non-standardized document layouts.

### Components 

1. **Document Ingestion Layer:** Uses `PyMuPDF` (Fitz) for high-performance extraction of raw text strings directly from binary data stream objects, preserving positional text layouts better than traditional extraction utilities.
2. **Deterministic Extraction Layer:** Implements optimized, boundary-isolated Regular Expressions (Regex) to target immutable structures such as complex international phone formats and RFC 5322 compliance-leaning email addresses.
3. **Semantic Phrase Matching:** Configures an optimized `PhraseMatcher` tracking custom vocabularies (e.g., industry-standard technical competencies) via lowercased token matching, enabling robust skill tracking independent of case variations.

4. ## 🛠️ Techn Stack

- **Python 3** 
- **Text Engine:** PyMuPDF (`fitz`)
- **NLP Ecosystem:** SpaCy Framework v3.x
- **Frontend Dashboard:** Streamlit
- **Python venv** 
