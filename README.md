# CampusSignals (CS216)

End-to-end analysis for **Cognitive & Behavioral Predictors of Student Outcomes** lives in [`analysis.ipynb`](analysis.ipynb).

## Setup

```bash
python -m venv .venv
source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install -r requirements.txt
```

Optional: copy [`.env.example`](.env.example) to `.env` for local API tokens (**never commit `.env`**).

## Data

- **Dataset A:** `datasets/mendeley/repositorio.xlsx` (or cached `datasets/mendeley/repositorio.csv` if present)
- **Dataset B:** `datasets/student-life/`

## Run

Open `analysis.ipynb`, pick the project interpreter / kernel, then **Run All** from the top (reproducibility seed is set near the start of the notebook).

Alternatively:

```bash
jupyter nbconvert --to notebook --execute --inplace analysis.ipynb
```

## Outputs

Key sections: Dataset A pipeline → Dataset B pipeline → cross-cohort comparison → robustness → diagnostics & limitations.
