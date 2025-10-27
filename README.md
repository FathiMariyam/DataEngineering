```markdown
# DataEngineering — Uber pickups quick analysis

This repository contains a single Jupyter notebook `Uber_analysis.ipynb` which performs a short exploratory analysis on a public Uber dataset (April 2014).

How to run
- Locally:
  - Python 3.9+ recommended.
  - Create and activate a virtual environment.
  - pip install -r requirements.txt
  - jupyter notebook and open `Uber_analysis.ipynb`.
- Colab:
  - Upload `Uber_analysis.ipynb` to Colab (File → Upload notebook) and run.
- CI:
  - A GitHub Actions workflow will run the notebook on pushes to `main` and store the executed notebook as an artifact.
- Docker:
  - Build: `docker build -t dataengineering-notebook .`
  - Run: `docker run -p 8888:8888 dataengineering-notebook` and follow Jupyter output.

Files added:
- `requirements.txt` — Python dependencies
- `.github/workflows/run-notebook.yml` — executes the notebook using papermill
- `Dockerfile` — container to run the notebook/Jupyter
- `README.md` — this file

Notes
- The notebook uses a public CSV hosted in the notebook; if you have additional data from the original repository, upload CSVs to the repo and update the path in `Uber_analysis.ipynb`.
- If you previously exposed a PAT, revoke it immediately (see message above).
```
