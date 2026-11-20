# College Student Expense Management System

A Python-based CLI application designed to help university students track their pocket money, categorize daily expenses, manage monthly budgets, and forecast month-end spending patterns.

Developed as part of the **Computational Thinking and Programming (2026CSAE100)** course at **Bennett University**.

---

## 🚀 Key Features

* **💰 Daily Expense Logging:** Record daily expenses with date, category, description, and amount with thorough input validation.
* **📊 Category-wise Analysis:** Real-time breakdown of expenses across categories (Food, Transport, Stationery, Entertainment, Academic, Other) with interactive terminal ASCII bar graphs.
* **⚠️ Multi-Tier Budget Monitoring:** 4-level rule-based budget status:
  * `SAFE`: Under 50% of budget used
  * `MODERATE`: 50% to 80% used
  * `WARNING`: 80% to 100% used (and spending equal to budget)
  * `OVER BUDGET`: Above 100% of budget
* **📈 Predictive Analytics & Projection:** Daily burn rate calculation and month-end spending projections that warn users before budget overruns occur.
* **🔍 Anomaly Detection:** Identifies days with unusual spending (days exceeding 2x the average daily spend).
* **📉 Chart Export:** Visualizes spending by category using Matplotlib with automatic fallback if the library is not installed.
* **💾 Data Persistence:** File-based data storage utilizing CSV (`expenses.csv`) and text (`budget.txt`) with automated corrupted row handling.

---

## 🛠 Project Structure

```text
├── main.py        # Central CLI interface, input validation, and system integration
├── analysis.py    # Analytical computation engine, ranking, and budget rules
├── storage.py     # File handling, CSV reading/writing, and data cleaning
├── .gitignore     # Git ignore configuration
└── README.md      # Project overview and documentation
```

---

## 💻 How to Run

### Prerequisites
* Python 3.8 or higher
* (Optional) `matplotlib` for chart generation (`pip install matplotlib`)

### Execution
Run the application from your terminal:
```bash
python3 main.py
```

---

## 👥 Team & Contributions

* **Tanmay Kaushik** (`S26CSEU1401`): Data persistence and storage layer (`storage.py`), add/view/delete options with input checks.
* **Parth Sahlot** (`S26CSEU1410`): Analytical computations, category sorting/ranking, and budget projection rules (`analysis.py`).
* **Vaibhav Ojha** (`S26CSEU1372`): System architecture, main CLI menu loop, integration, edge-case testing, and report compilation (`main.py`).

**Faculty Mentor:** Jayant Vyas
