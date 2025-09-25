
For VM:
-----------
python -m venv venv

.\venv\Scripts\activate

pip install python-dotenv requests pandas numpy sentence-transformers faiss-cpu fastapi pydantic streamlit

python -m ensurepip --upgrade

pip install python-dotenv requests pandas numpy sentence-transformers faiss-cpu fastapi pydantic streamlit

streamlit run frontend/streamlit_app.py


Non-VM:
-----------
# AI Insurance FAQ RAG Project

## Prerequisites
- Python 3.8+
- pip

## Installation
1. Open a terminal in the project root (`D:\AI_Workspace\AILab_Non_VM`).
2. Install required packages:
   ```powershell
   pip install -r requirements.txt
   pip install -r frontend/requirements.txt
   pip install faiss-cpu streamlit python-dotenv
   ```

## Running the Backend (FastAPI)
1. In the project root, run:
   ```powershell
   python -m backend.main
   ```
2. The API will be available at: [http://127.0.0.1:8000](http://127.0.0.1:8000)

## Running the Frontend (Streamlit)
1. Open a new terminal in the project root.
2. Run:
   ```powershell
   streamlit run frontend/streamlit_app.py
   ```
3. The app will open in your browser.

## Notes
- Ensure `data/faqs.csv` exists for default ingestion.
- If you encounter missing package errors, install them using `pip install <package-name>`.

## Project Structure
- `backend/` - FastAPI backend scripts
- `frontend/` - Streamlit frontend app
- `data/` - CSV data files
- `index_store/` - Index files

---
For any issues, check the terminal output for error messages and ensure all dependencies are installed.

python -m backend.main

streamlit run frontend/streamlit_app.py

