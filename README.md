# WLDUSDT 1-Minute Historical Kline Dataset

An institutional-grade, open-source archive of cleaned, standardized, and validated **1-minute intraday historical kline data** for **WLDUSDT** (Binance Spot).

---

## 📊 Dataset Specifications
- **Symbol:** `WLDUSDT`
- **Market:** Binance Spot
- **Timeframe:** 1 Minute (`1m`)
- **Total Months:** `40` months
- **Total Candles:** `1,701,540` 1-minute candles
- **Historical Range:** `2023-07-24 09:00:00` to `2026-10-17 23:59:00` (UTC)
- **Schema:** `timestamp, datetime_utc, open, high, low, close, volume, quote_volume, trade_count, taker_buy_volume, taker_buy_quote_volume`

---

## 🏛️ Directory Hierarchy
```text
WLDUSDT-Historical-Data/
├── README.md
└── 1m/
    └── <YYYY>/
        └── <MM>/
            └── WLDUSDT_1m_<YYYY-MM>.csv
```

---

## ⚡ 1-Line Pandas Stream Loader
Load any month directly from GitHub's raw CDN without cloning the repository:

```python
import pandas as pd

url = "https://raw.githubusercontent.com/parshant231234-eng/WLDUSDT-Historical-Data/main/1m/2026/10/WLDUSDT_1m_2026-10.csv"
df = pd.read_csv(url)
print(df.head())
```
