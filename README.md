
# Wings R Us – Recommendation System
## Team: Data Achievers
---

---

## 📌 Objective
Build a personalized recommendation system to predict the missing item in a customer's order cart based on past order history. The goal is to enhance customer experience and increase basket size using smart last-minute suggestions.

---

## 📂 Contents

- `wwt_recommendation.ipynb`: Complete data pipeline from loading, cleaning, rule mining, and prediction.
- `requirements.txt`: Required packages to run the notebook.
- `WWT_ChickenMasters_Output.xlsx`: Final predictions for the test data.
- `ChickenMasters_Presentation.pptx`: Business and technical presentation.
- `README.md`: This file.

---

## 🧠 Approach

- **Algorithm Used**: Apriori Association Rule Mining
- **Cleaning**: Removed noisy items (e.g., 'Order Memo', 'Blankline')
- **Basket Generation**: Extracted cleaned item lists per order
- **Sampling**: 25,000 baskets used to prevent memory overflow
- **Rule Mining**: Confidence × Lift based ranking for item prediction
- **Prediction Logic**: For each test cart with 3 items, recommend top 3 missing items using high-confidence rules

---

## 📈 Evaluation

- Metric: **Recall@3**
- For each test order, if the true missing item is in the top 3 predictions → counted as correct.

---

## 🚀 Deployment Notes

- The solution is scalable across Wings R Us mobile app, website, and kiosks.
- Ideal for A/B testing or limited rollout in one store with analytics tracking.

---

## 👨‍💻 Team Members
- [Your Name(s)]
- [Email(s)]
- [GitHub / LinkedIn (Optional)]

---
