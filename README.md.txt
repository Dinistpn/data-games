# 🎮 Video Game Market & Revenue Analytics

An end-to-end data analytics and business intelligence project exploring global video game performance, revenue drivers, pricing strategies, and customer segmentation using Python and Power BI.

---

## 📌 Project Overview

Understanding what drives revenue and user satisfaction in the gaming industry is critical for studios, publishers, and market analysts. This project analyzes transactional video game data to uncover pricing patterns, evaluate genre profitability, and group titles into actionable business clusters using unsupervised machine learning.

### Key Objectives
- **Exploratory Data Analysis (EDA):** Identify revenue distributions, top-performing genres, and publisher trends.
- **Machine Learning (K-Means Clustering):** Segment games into four distinct market tiers based on pricing, sales volume, and user scores.
- **Business Intelligence (Power BI):** Build an interactive multi-page dashboard for dynamic scenario tracking and executive reporting.

---

## 🛠️ Project Architecture & Tech Stack

- **Data Processing & ML:** Python (`Pandas`, `NumPy`, `Scikit-learn`)
- **Data Visualization:** Power BI Desktop (DAX, Power Query)
- **Environment:** Kaggle Notebooks, Jupyter Notebook, GitHub

```text
data-games/
├── CITATIONS.md                 # Standalone dataset attribution & licensing
├── README.md                    # Main project documentation
├── data/
│   ├── raw_games.csv            # Original dataset from Kaggle
│   └── cleaned_games.csv        # Processed dataset with engineered metrics & ML clusters
├── notebooks/
│   └── game_analysis.ipynb      # Complete Python EDA & K-Means clustering script
└── power_bi/
    └── steam_analytics.pbix     # Interactive Power BI report dashboard
📊 Methodology & Analytical Pipeline
1. Data Cleaning & Feature Engineering
Imputed missing user ratings and pricing values.

Categorized prices into discrete market brackets: Free to Play, Budget (<$20), Mid-Tier ($20–$50), and AAA / Premium ($50+).

Calculated derived business metrics including total_revenue = price * units_sold.

2. Machine Learning Segmentation (K-Means)
Using scaled numerical features (price, user_score, and units_sold), games were grouped into 4 strategic clusters:

Blockbuster Hits: High revenue, high sales volume, and strong user ratings.

Niche / High Score: Highly rated titles with moderate to boutique sales numbers.

Budget / Casual: Lower-priced titles relying on volume sales.

Underperforming: Games with low ratings or stagnant sales trajectories.

3. Business Intelligence (Power BI Dashboard)
Executive Summary: High-level KPI cards, revenue trends over time, and top-performing game lists.

Publisher & Genre Drill-Down: Matrix views and dynamic slicers for deep-dive regional and genre analysis.

Decomposition Tree: Interactive root-cause visual breaking down total sales across platforms and publishers.

Clone the Repository:

Bash
git clone [https://github.com/Dinistpn/data-games.git](https://github.com/Dinistpn/data-games.git)
cd data-games
Execute Python Analysis:

Open notebooks/game_analysis.ipynb in Jupyter Notebook or VS Code.

Run all cells to process the data and output the transformed dataset to data/cleaned_games.csv.

Open Power BI Dashboard:

Launch Power BI Desktop.

Open power_bi/steam_analytics.pbix.

If prompted, update the data source path to point to your local data/cleaned_games.csv.


---

### How to Add This to Your Repository

1. On your GitHub repo page (`[https://github.com/Dinistpn/data-games](https://github.com/Dinistpn/data-games)`), click the **`README.md`** file (or click **Add file** $\rightarrow$ **Create new file** and name it `README.md`).
2. Click the **pencil icon** (✏️) to edit.
3. Paste the markdown text above into the editor.
4. Click **Commit changes...** at the top right.

<ElicitationsGroup message="What would you like to set up next for your repo?">
  <Elicitation label="Draft a CITATIONS.md file for the repo" query="Draft a CITATIONS.md file formatted for the Dinistpn/data-games repository."/>
  <Elicitation label="Help writing Git commands to upload local files" query="Show me the Git CLI commands to push my local files into the Dinistpn/data-games repository."/>
</ElicitationsGroup>
