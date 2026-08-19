# AI Resume Evaluator

A Flask web app (Internie.pk GenAI internship task) that extracts text from **PDF/DOCX** resumes and asks **Groq** (via LangChain) for structured feedback on strengths, gaps, and improvements.

## Technology stack

- Python, Flask
- pdfplumber, python-docx
- LangChain, Groq

There is no Streamlit app in this repository.

## Installation

```bash
git clone https://github.com/hamza2324/resume-evaluator-tool.git
cd resume-evaluator-tool
python -m venv .venv
source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install -r requirements.txt
```

## Configuration

```env
GROQ_API_KEY=your_groq_api_key_here
```

See `config.py` for how the key is loaded. Do not commit secrets. `__pycache__/` and `uploads/` should be gitignored.

## Usage

```bash
python app.py
```

## License

MIT — see `LICENSE`.
