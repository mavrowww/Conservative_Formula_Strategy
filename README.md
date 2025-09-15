# Conservative Formula Strategy

A quantitative investing project that implements and analyzes the **Conservative Formula** strategy,
originally proposed by *Pim van Vliet & David Blitz (2018)*.

This project replicates and tests the strategy on the **S&P 500 universe**,
selecting stocks based on three factors:

- **Momentum** (12–1 month returns, skipping the most recent month)
- **Low Volatility** (36-month rolling volatility of returns)
- **Dividend Yield** (used as a proxy for Net Payout Yield due to limited data availability)

The portfolio is rebalanced quarterly, with **100 equally-weighted stocks** selected each period.

---

## Project Structure
- `Conservative_Formula_Strategy.ipynb` → main Jupyter Notebook with code, analysis, plots, and interpretation  
- `requirements.txt` → Python dependencies (pandas, numpy, matplotlib, yfinance, tqdm, scipy, jupyter, ipywidgets)  

---

## Key Results
- Backtests show consistent outperformance versus benchmarks (SPY, IWM)  
- Lower volatility and drawdowns compared to market indices  
- Higher risk-adjusted returns (Sharpe ratio above benchmarks)  
- Results account for transaction costs  

*(Exact figures such as CAGR, Sharpe ratio, and Max Drawdown are provided in the notebook.)*

**Cumulative Total Return (backtest period):**

| Strategy   | Total Return |
|------------|--------------|
| Portfolio  | **719.46%**  |
| SPY        | 659.04%      |
| IWM        | 360.37%      |


![Cumulative NAV — Conservative Formula vs Benchmarks](https://github.com/user-attachments/assets/79b8945e-89a0-4339-a644-8abe88aa82a6)

![Portfolio Calendar-Year Returns](https://github.com/user-attachments/assets/2b1c0784-8594-4eb4-91ad-ec3db2499b39)


## View the Notebook

- [View on nbviewer](https://nbviewer.org/github/mavrowww/Conservative_Formula_Strategy/blob/main/Conservative_Formula_Strategy.ipynb?flush_cache=true)  
- [Open in Google Colab](https://colab.research.google.com/github/mavrowww/Conservative_Formula_Strategy/blob/main/Conservative_Formula_Strategy.ipynb)


---

## Installation & Usage

Clone the repository:
```bash
git clone https://github.com/mavrowww/Conservative_Formula_Strategy.git
cd Conservative_Formula_Strategy
```

Install dependencies (Python 3.9+ recommended):
```bash
pip install -r requirements.txt
```

Run the Jupyter notebook:
```bash
jupyter notebook Conservative_Formula_Strategy.ipynb
```

## References
- Pim van Vliet & David Blitz (2018). [*The Conservative Formula: Quantitative Investing Made Easy*](https://ssrn.com/abstract=3145152)  
- Van Vliet & Jan de Koning (2017). *High Returns from Low Risk* (Wiley)

---

## Disclaimer
This project is for **educational and analytical purposes only**.
It does **not** constitute financial advice or investment recommendations.

All analysis and code are original implementations based on publicly available research and historical data.