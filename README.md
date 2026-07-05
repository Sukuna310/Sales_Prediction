# 📊 Sales Prediction Project

Ever wondered how much you'd sell if you spent a certain amount on ads? This project answers that question using machine learning!

## 🎯 What It Does

Predicts product **sales** based on advertising budget spent across three channels:
- 📺 **TV** - Television advertising
- 📻 **Radio** - Radio advertising  
- 📰 **Newspaper** - Print advertising

## 🚀 Quick Start

```bash
# Open the notebook
jupyter notebook "Sales Prediction.ipynb"
```

That's it! Run all cells to see the magic happen.

## 📈 The Data

We use the classic Advertising dataset with 200 records:
- Each row = one market/campaign
- Features: TV, Radio, Newspaper ad spend (in thousands of dollars)
- Target: Sales (in thousands of units)

| Channel | Avg Spend | Range |
|---------|-----------|-------|
| TV | $147K | $0.7K - $296K |
| Radio | $23K | $0 - $50K |
| Newspaper | $31K | $0.3K - $114K |

## 🤖 Models Used

| Model | R² Score | Verdict |
|-------|----------|---------|
| Linear Regression | 0.899 | Solid baseline |
| Random Forest | 0.981 | Pretty good! |
| **Gradient Boosting** | **0.983** | 🏆 Best performer |

### Key Findings

1. **Radio ads work best** — Each dollar in radio brings ~$0.19 in sales
2. **TV ads have steady returns** — ~$0.04 per dollar spent
3. **Newspaper? Barely moves the needle** — Only ~$0.003 per dollar!

The correlation heatmap shows Radio has the strongest relationship with Sales, followed by TV. Newspaper? You're better off saving your money.

## 📁 Project Structure

```
Sales_Prediction/
├── Sales Prediction.ipynb    # Main analysis & models
└── Datasets/
    └── Advertising.csv       # Raw data
```

## 🛠️ Tools Used

- **Pandas** — Data wrangling
- **NumPy** — Number crunching
- **Matplotlib & Seaborn** — Beautiful visualizations
- **Scikit-learn** — Machine learning models

## 💡 What I Learned

- Gradient Boosting outperformed both Linear Regression and Random Forest
- Cross-validation showed consistent results (low variance = reliable models)
- The TV × Radio interaction term could boost Linear Regression performance

---


