## Setup Instructions

### Prerequisites
- Python 3.8+
- pip

### Installation

1. Clone the repository:
```bash
git clone https://github.com/YOUR_USERNAME/counter-uas-market-analysis.git
cd counter-uas-market-analysis
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Download data:
- Go to USASpending.gov
- Search: "counter UAS" OR "counter unmanned"
- Download Award-level data
- Save CSV to `data/` folder as `Contracts_PrimeAwardSummaries_2026-01-09_H17M01S51.csv`

4. Run analysis:
```bash
jupyter notebook
# Open notebooks/01_explore_data.ipynb
```

## Project Structure
```
counter-uas-market-analysis/
├── data/                  # Raw data (not in git)
├── notebooks/             # Jupyter notebooks
├── scripts/               # Python scripts
├── output/                # Charts and results
├── README.md
└── requirements.txt
```
```

---

### 4. **Update Your `.gitignore`**

Make sure your `.gitignore` includes:
```
# Data files
data/*.csv

# Python
__pycache__/
*.py[cod]
.ipynb_checkpoints/
venv/
env/

# OS specific
.DS_Store      # Mac
Thumbs.db      # Windows
*.swp          # Linux

# Jupyter
.ipynb_checkpoints/

# Environment
.env