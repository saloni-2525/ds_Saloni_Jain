# Trader Behaviour vs Market Sentiment

This project explores how trader performance changes when the market sentiment
is in Fear, Greed, or Neutral mode. I combined the trading dataset with the
Bitcoin Fear & Greed Index to see how things like PnL, win rate, and trading
volume behave under different moods of the market.

---

## Project Structure

ds_saloni_jain/
│
├── notebook_1.ipynb      # Main analysis
├── csv_files/            # Input data
├── outputs/              # Saved charts
└── ds_report.pdf         # Summary report

---

## What I Did

- Cleaned both datasets and converted timestamps
- Merged trades with sentiment using the date
- Calculated:
  - Average PnL
  - Win rate
  - Trading volume
  - Buy vs Sell counts
- Created visualizations for these metrics
- Did a simple KMeans clustering on trader behavior
- Added a small pipeline demo showing how data could be prepared for ML
- Checked how PnL behaves during sentiment shifts (like Fear → Greed)

---

## Key Takeaways

- Greed days had the highest PnL and the most trading activity
- Win rate was only slightly better in Greed
- Fear seemed more cautious
- Neutral performed the worst
- Clustering showed different types of traders (safe, aggressive, risky)
- Sentiment flips can be more volatile than steady phases

---

## How to Run

1. Open `notebook_1.ipynb` in Google Colab
2. Mount Google Drive
3. Make sure paths match your folder
4. Run all cells top to bottom

Libraries used: pandas, numpy, matplotlib, seaborn, scikit-learn

---

## Note

There was no leverage column in the dataset, so leverage wasn't analyzed.

The historical_data.csv file is large, so it is stored on Google Drive:
[Click here to access the dataset](https://drive.google.com/file/d/1Gw-QK9wVAo2Df6X_lpCn3tYSwKraCrYT/view?usp=sharing)
---

## Author

**Saloni Jain**
