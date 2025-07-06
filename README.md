# ⚡ Energy Policy Causal Analysis using Machine Learning

This project evaluates the **causal impact of energy policy incentives** (such as support for Solar and Wind power plants) on actual electricity generation using advanced **causal machine learning techniques** like **Double Machine Learning (DML)** and **Causal Forests**.

---

## 🎯 Objective

To estimate the **Average Treatment Effect (ATE)** of energy policy incentives on electricity generation in 2017 using:
- ✅ Double Machine Learning (DML)
- ✅ Causal Forest DML

---

## 📊 Dataset

- **Source**: Global Power Plant Database
- **Size**: 36 columns, ~33,000 rows
- **Key Variables**:
  - `primary_fuel` (Solar, Wind, Hydro, etc.)
  - `capacity_mw`
  - `estimated_generation_gwh_2017`
  - **Derived Feature**: `policy_incentive` (1 = Solar/Wind, 0 = Others)

---

## 🧠 Methods Used

- 🔍 Data Cleaning & Feature Engineering
- 📈 Exploratory Visualization (e.g., bar chart comparison)
- 🤖 Causal Machine Learning using `econml`:
  - `LinearDML` with LassoCV and Random Forest
  - `CausalForestDML` for heterogeneous treatment effects

---

## 🧪 Results Summary

- 📌 **Double Machine Learning ATE**: `-306.31 MWh`
- 📌 **Causal Forest ATE**: `-325.80 MWh`

These values suggest that, on average, **renewable energy plants (solar/wind)** generated slightly **less electricity** than non-supported plants in 2017 — likely due to their smaller size and newer installations.

---

## 🛠️ Tools & Libraries

- **Language**: Python (Jupyter Notebook)
- **Libraries Used**:
  - `pandas`, `numpy`
  - `matplotlib` (for visualization)
  - `scikit-learn` (for models and preprocessing)
  - `econml` (for causal inference models)

---

## 🗂️ Repository Structure

