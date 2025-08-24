# LangChain Document Loader Lab

This repository contains a Jupyter notebook demonstrating how to use the
document loading utilities in the [LangChain](https://python.langchain.com)
ecosystem.  The lab walks through loading content from a variety of
sources—plain text, PDFs, Markdown, JSON, CSV, web pages, Word documents,
and unstructured files—and shows how each loader produces a `Document`
object that can be passed to downstream processing tools.

## Contents

| File | Description |
| --- | --- |
| `LangChain_document_loader.ipynb` | The lab notebook with step‑by‑step examples for each loader type. |
| `requirements.txt` | Pinned Python dependencies required to run the notebook. |

## Getting Started

To run the notebook locally in VS Code or another Jupyter environment:

1. **Clone the repository** to your machine:

   ```bash
   git clone <repo-url>
   cd langchain_document_loader_lab
   ```

2. **Create and activate a virtual environment** (recommended):

   ```bash
   python3 -m venv .venv
   source .venv/bin/activate  # on Windows use .venv\Scripts\activate
   ```

3. **Install the dependencies** from `requirements.txt`:

   ```bash
   pip install --upgrade pip
   pip install -r requirements.txt
   ```

4. **Launch the notebook**. In VS Code, open the folder and run
   `LangChain_document_loader.ipynb` using the Python interpreter from
   your virtual environment. Alternatively, start Jupyter from the
   command line:

   ```bash
   jupyter notebook LangChain_document_loader.ipynb
   ```

## Notes

* Several cells in the notebook download example files from IBM’s public
  course repository using `wget`. When running the notebook, ensure
  you have an internet connection or replace the URLs with locally
  accessible files.

* Optional exercises at the end of the notebook require additional
  packages (`arxiv` and `pypdfium2`), which are included in the
  `requirements.txt` for convenience.

* The lab notebook suppresses warnings for readability; feel free to
  remove the warning suppression if you wish to see more detailed
  output from underlying libraries.