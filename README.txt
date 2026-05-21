# Early Game Indicators in Professional League of Legends

A data science project analysing professional League of Legends esports match data to identify which early-game indicators most reliably predict the match winner.

**Course:** COMP-248 Project in Data Science  
**Author:** George Andreou  
**University of Nicosia**

---

## Project Overview

This project investigates how strongly early-game events (within the first 15 minutes) predict the eventual winner of professional League of Legends matches. The analysis covers three seasons (2019, 2022, 2025) across the five main competitive regions (LCK, LPL, LEC, LCS, PCS), totalling **53,882 team-level match rows**.

### Research Questions

1. Which early-game stats are most linked to winning?
2. How reliably do early indicators forecast match outcomes?
3. Does the importance of these metrics change across seasons?
4. Do different regions show different early-game patterns?

---

## Key Findings

1. **Objective Hierarchy** — Tower-based objectives (78%+ win rate) outperform kill- and dragon-based objectives (~60%). First to three towers is nearly as strong a predictor as first baron.

2. **Combined Early Score Scales Linearly** — A team winning 0/5 early indicators wins 13.7% of games; winning all 5 indicators wins 86.3%. The 2→3 jump is the threshold that flips a team from underdog to favourite.

3. **Gold Lead is the Universal Premium** — Within every score level, having a gold lead at 15 minutes is worth a constant **+27 percentage points** of win rate. First blood paired with gold lead adds zero additional value; first tower adds +11pp; first dragon adds +15.5pp.

4. **Baron is the Conversion Mechanism** — Teams ahead in gold but without first baron win only 44.5%. Securing baron raises that to 91.9%. Teams BEHIND in gold who steal baron win 70.7% — a 62-point swing making baron the single most powerful comeback tool.

5. **Side Advantage** — Blue side wins 52.8% of games, driven by herald (+18pp) and tower (+9pp) control. The effect is strongest in Western regions (+9pp) and smallest in LCK/LPL (+2-3pp).

6. **Objective Decay** — All early indicators lose predictive power past 35 minutes. Only inhibitor (72% win rate at 40+ min) retains decisive power in long games.

---

## Repository Structure
lol early game analysis/
├── inspectDataLol.ipynb           # Main analysis notebook
├── README.md                    # This file
├── Final_Report.pdf             # 3-page final report
├── data/
│   ├── 2019_LoL_esports_match_data_from_OraclesElixir.csv
│   ├── 2022_LoL_esports_match_data_from_OraclesElixir.csv
│   └── 2025_LoL_esports_match_data_from_OraclesElixir.csv
└── presentations/
├── Milestone1.pdf
└── Milestone2.pptx

---

## Tools & Technologies

- **Python 3** with pandas and numpy for data manipulation
- **Matplotlib** for visualisation
- **Jupyter Notebook** for analysis
- **Oracle's Elixir** for professional LoL match data

---

## How to Run

1. Clone the repository:git clone https://github.com/Geoand02/lol early game analysis.git
2. Install dependencies:pip install pandas numpy matplotlib jupyter
3. Launch Jupyter from the repository folder:jupyter notebook4. Open `inspectData.ipynb` and run all cells.

---

## Data Source

All match data is from [Oracle's Elixir](https://oracleselixir.com), a free public dataset of professional League of Legends matches. The CSVs included are unmodified from the original source.

---

## Project Video

[]

