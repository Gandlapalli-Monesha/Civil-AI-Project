# 🏗️ AI-Based Partition Wall Performance Predictor

An AI-powered tool to **predict structural performance and optimize material usage** in patterned concrete partition walls.

---

# 📌 Project Overview

Modern architectural partition walls often use **internal geometric patterns (infill)** instead of solid concrete to:

* Reduce material usage
* Lower cost
* Improve sustainability
* Maintain structural strength

However, testing each design physically is expensive and time-consuming.

## 💡 Solution

This project uses **Machine Learning (Random Forest)** to:

> Predict stress and stiffness of a wall design **before it is built**

and help identify designs that are:

* Strong enough
* Material-efficient

---

# 🎯 Objectives

* Predict structural performance of patterned walls
* Reduce reliance on physical testing
* Enable faster design decisions
* Optimize material usage (cement reduction)

---

# 🧠 How It Works

```text
Input Design Parameters → ML Model → Predicted Performance
```

### Inputs (User-defined):

* Pattern type (Honeycomb, Grid, etc.)
* Porosity
* Filament thickness
* Void area
* Number of joints
* Geometry parameters
* etc.

### Outputs (Predicted):

* Maximum Stress (Z & Y directions)
* Relative Stiffness (Z & Y directions)

---

# ⚙️ Tech Stack

* **Python**
* **Pandas** – data handling
* **Scikit-learn** – ML model (Random Forest)
* **Streamlit** – UI
* **Joblib** – model saving/loading

---

# 🤖 Machine Learning Model

* Model: **Random Forest Regressor**
* Type: **Multi-output regression**
* Validation: **Leave-One-Out Cross Validation**

## Why Random Forest?

* Works well with small datasets
* Handles nonlinear relationships
* Provides feature importance

---

# 📊 Key Insight

The model learns relationships like:

* Geometry → stiffness
* Porosity → material reduction
* Void structure → stress behavior

---

# 📈 Sample Results

| Output            | Performance                |
| ----------------- | -------------------------- |
| Stiffness Z       | ✅ High accuracy (~0.74 R²) |
| Stress Prediction | ⚠️ Moderate (limited data) |

---

# 🧱 Engineering Perspective

This project solves:

```text
Maximize Strength / Stiffness  
Minimize Material Usage
```

---

# 💻 UI (Streamlit App)

The application provides:

* Interactive parameter inputs
* Real-time predictions
* Performance interpretation
* Clean visualization

### Run the app:

```bash
python -m streamlit run app.py
```
---

# 🚀 How to Use

## 1. Train Model

```bash
python Code/train.py
```

## 2. Run App

```bash
python -m streamlit run Code/app.py
```

---

# ⚠️ Limitations

* Small dataset (~20 samples)
* Stress predictions less accurate than stiffness
* Real-world validation still required

---

# 🔮 Future Improvements

* Increase dataset size
* Add optimization engine (best design suggestion)
* Improve stress prediction accuracy
* Integrate CAD/geometry input
* Add cost + carbon footprint estimation

---

# 🧩 Applications

* Architectural design
* Lightweight construction
* Sustainable building systems
* 3D printed concrete structures

---

# 📌 Conclusion

This project demonstrates how AI can:

> Assist in designing **material-efficient yet structurally reliable** partition walls

reducing cost, time, and environmental impact.

---

# 👩‍💻 Author
Gandlapalli Monesha.

Built as part of a Civil + AI interdisciplinary project.

---

