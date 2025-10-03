# E-commerce Market Basket Analysis

## 📖 Overview

This project analyzes a transactional dataset from a UK-based online retailer to uncover hidden associations between products. The primary goal is to identify which items are frequently purchased together and leverage this information to develop actionable business strategies for increasing sales and improving customer experience.

The analysis uses the **Apriori algorithm**, a fundamental technique in Market Basket Analysis, to generate association rules and identify significant purchasing patterns.

---

## 📊 Dataset

The data used is the [Online Retail Data Set](http://archive.ics.uci.edu/ml/datasets/Online+Retail) from the UCI Machine Learning Repository. It contains all the transactions occurring between 12/01/2010 and 12/09/2011 for a UK-based and registered non-store online retail.

---

## 🎯 Key Questions Addressed

1.  What are the most frequent itemsets purchased by customers?
2.  What are the strongest association rules between products?
3.  How can we translate these data-driven insights into concrete business strategies?

---

## 🛠️ Tools and Libraries

*** **Python 3.13**
* **Pandas:** For data cleaning and manipulation.
* **mlxtend:** For implementing the Apriori algorithm and generating association rules.
* **Matplotlib & Seaborn:** For data visualization.
* **NetworkX:** For creating a network graph of product associations.

---

## ⚙️ How to Run

1.  Clone the repository:
    ```bash
    git clone [https://github.com/your-username/your-repo-name.git](https://github.com/your-username/your-repo-name.git)
    ```
2.  Install the required libraries:
    ```bash
    pip install pandas mlxtend matplotlib seaborn networkx openpyxl
    ```
3.  Place the `Online Retail.xlsx` dataset in the project's root directory.
4.  Run the Jupyter Notebook or Python script to perform the analysis.

---

## ✨ Key Findings & Visualizations

The analysis successfully identified several strong purchasing patterns. The "best" rules were identified as those with high **lift**, **confidence**, and **support**.

### Finding 1: Customers Collect Product Sets
The strongest associations were found among items that belong to a larger collection. For example, the **"POPPY'S PLAYHOUSE"** items (Livingroom, Bedroom, Kitchen) were almost always purchased together.

### Finding 2: Customers Buy Coordinated Themes
Beyond formal sets, items sharing a common theme, like the **"SCANDINAVIAN CHRISTMAS"** decor, were also frequently purchased in the same transaction.

## 🚀 Actionable Recommendations

Based on the findings, the following business strategies are recommended:

1.  **Implement Product Bundling:** Create a **"Poppy's Playhouse Complete Set"** bundle with a small discount to encourage customers to purchase the entire collection at once.
2.  **Enhance Thematic Cross-Selling:** Develop curated landing pages like a **"Scandinavian Christmas Collection"** and use targeted pop-ups to recommend related items when a customer adds a themed product to their cart.
3.  **Launch Multi-Buy Promotions:** For items often bought in different colors (e.g., small bowls), run promotions like **"Buy any 2, get the 3rd 50% off"** to increase the number of items per transaction.
