# Bangalore Home Price Prediction

This project is a **full-stack end-to-end machine learning solution** that predicts housing prices in Bangalore, India, based on multiple property features. It showcases my ability to work across the full ML pipeline: from data cleaning and feature engineering, to model development and deployment via a RESTful API.

---

## 🔧 Project Features

* **Exploratory Data Analysis (EDA)**: Comprehensive data cleaning, outlier removal, feature engineering and visualization.
* **Machine Learning**: Linear Regression model for price prediction, trained on pre-processed and engineered features.
* **Model Evaluation**: Evaluation of model performance using cross-validation and GridSearchCV techniques.
* **API Deployment**: Model served via Flask REST API for real-time prediction.
* **Code Modularity**: Clean, modular codebase with helper utilities (`utils.py`) and API backend (`server.py`).
* **Reproducible Notebook**: Complete Jupyter Notebook (`bangolare_home_prices.ipynb`) showcasing the entire ML workflow.

---

## 📊 Dataset

The dataset consists of real-world Bangalore housing price data which was gotten from Kaggle. Key features used:

* Location
* Total Square foot
* Number of bedrooms (BHK)
* Number of bathrooms
* Price

---

## 📉 ML Workflow Summary

1. **Data Cleaning:**

   * Handled missing values, data type inconsistencies and text-based square footage inputs.
   * Normalized multi-format area strings (e.g. "2100-2850 sqft") into numeric averages.

2. **Feature Engineering:**

   * Created new features such as `price_per_sqft` for better modeling.
   * Handled rare locations via dimensionality reduction to avoid sparse one-hot encoding.

3. **Outlier Detection & Removal:**

   * Applied domain-driven thresholds to remove unrealistic data points.

4. **Model Training:**

   * Linear Regression model trained on cleaned and engineered data.
   * Hyperparameter tuning and cross-validation for robustness.

5. **Model Deployment:**

   * Trained model saved as pickle file.
   * Flask-based API server built to serve real-time predictions.

---

## 🔬 Technologies Used

* Python
* Pandas, NumPy
* Matplotlib, Seaborn
* Scikit-learn
* Flask (for REST API)
* Jupyter Notebook


---

## 🔧 How to Run the Project

### 1. Clone the repository

```bash
git clone <repo_url>
cd server
```

### 2. Install dependency

```bash
pip install Flask
```

### 3. Run Jupyter Notebook (optional)

```bash
jupyter notebook
# Open bangalore_home_prices.ipynb
```

### 4. Start the Flask API server

```bash
python server.py
```

The API will be available at: `http://127.0.0.1:5000/`

---

## 🌟 Why This Project Matters

* Demonstrates full ML lifecycle: **EDA → Feature Engineering → Model Training → Deployment**
* Combines strong **data cleaning and feature engineering** techniques (including custom parsers for complex area formats)
* Shows understanding of **API development**
* Modular, production-ready code base
* Real-world problem solving with messy data
## 🎓 About Me

I am a highly motivated reseacher, data scientist and software engineer with a passion for solving real-world problems through data-driven solutions. My projects combine deep data understanding with clean software engineering and deployment skills.

I am actively looking for opportunities in Research, Data Science, ML Engineering, and Full-Stack roles.

Let's connect!

* [LinkedIn](https://www.linkedin.com/in/joshua-owusu-ansah/)
* [GitHub](https://github.com/Joshua-123-ansah)

---

## 🚀 Future Improvements

* Incorporate non-linear models (Random Forest, XGBoost)
* Build a front-end UI to consume the deployed API
* Deploy the API on cloud platforms (Heroku, AWS, Azure)
* Containerize with Docker for production deployment

---
