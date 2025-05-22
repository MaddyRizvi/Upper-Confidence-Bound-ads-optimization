# 🎯 Upper Confidence Bound (UCB) - Reinforcement Learning on Ad Click Simulation

## 📌 Summary

This project implements the **Upper Confidence Bound (UCB)** algorithm, a reinforcement learning approach used to solve the **Multi-Armed Bandit** problem. The UCB strategy is applied to a simulated advertisement click dataset to optimize ad selection by maximizing click-through rates (CTR). The algorithm balances **exploration** (trying new ads) and **exploitation** (focusing on ads known to perform well), making it a practical solution for ad placement and recommendation systems.

---

## 📂 Dataset

The dataset used in this project is `Ads_CTR_Optimisation.csv`, which simulates user behavior with 10 different ads. Each row represents a round (user session), and each column represents an ad. The values are binary:
- `1`: User clicked on the ad
- `0`: User did not click

This binary feedback forms the basis for the reinforcement learning algorithm to make smarter decisions over time.


## 📁 Repository Structure

- `apriori_analysis.py` – Main script implementing UCB algorithm
- ` Ads_CTR_Optimisation.csv` – Simulated dataset of ad click responses
- `README.md` – Project overview and setup instructions
- `CONTRIBUTING.md` – Guidelines for contributors
- `requirements.txt` # Python dependencies


## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/MaddyRizvi/Upper-Confidence-Bound-ads-optimization.git
cd Upper-Confidence-Bound-ads-optimization
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

Or install individually:

```bash
import numpy as np 
import matplotlib.pyplot as plt
import pandas as pd
import math
```

### 3. 🚀 How to Run

Make sure your dataset is in the correct format, then run:

```bash
python upper_confidence_bound.py
```

---



## 📈 Output

The script will output:

- A visual histogram showing how many times each ad was selected

- Printed results for total reward (number of clicks)

- Insights on which ad performed best over time


## ⚙️ Details

- Algorithm: Upper Confidence Bound (UCB)

- Problem: Multi-Armed Bandit

- Distance Metric: Based on average reward and confidence interval:

## 🧠 Understanding

The UCB algorithm intelligently balances:

- Exploration: Selecting ads not shown often to gather more data.

- Exploitation: Selecting ads that have historically high click rates.

- Over time, this leads to improved ad selection decisions that maximize overall CTR.


## 📜 License

This project is licensed under the MIT License.


## 🤝 Contributions

Contributions are welcome! Please refer to the [CONTRIBUTING.md](./CONTRIBUTING.md) file for more details.
