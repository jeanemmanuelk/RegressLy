# RegressLy - Interactive Regression Analysis Application

## 📊 Overview
RegressLy is a powerful and user-friendly regression analysis application designed to simplify data-driven decision-making for users of all technical backgrounds. Built with Python and Streamlit, RegressLy allows seamless data upload, model selection, and interactive visualization to generate actionable insights without needing advanced programming skills.

## 🚀 Key Features
- **Automated Data Preprocessing:** Cleans data, removes outliers (z-score), scales features, and encodes categorical variables automatically.
- **Multiple Regression Models:** Supports Linear Regression, Random Forest, Ridge, Lasso, and ElasticNet for flexible modeling.
- **Interactive Visualizations:** Real-time feature importance and regression plots for intuitive data interpretation.
- **Performance Metrics Dashboard:** Displays MAE, MSE, RMSE, and R² Score for evaluating model performance.
- **User-Centric Interface:** Streamlit-based design for effortless navigation and analysis.

## 🛠️ Tech Stack
- **Frontend:** Streamlit
- **Backend:** Python
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, SciPy, Scikit-learn

## 📥 Installation
1. **Clone the Repository:**
   ```bash
   git clone https://github.com/jeanemmanuelk/RegressLy.git
   cd RegressLy
   ```

2. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the App:**
   ```bash
   streamlit run app.py
   ```

## 💡 Usage Guide
1. **Upload Dataset:** Use the sidebar to upload a CSV dataset.
2. **Select Target Variable:** Choose the column to predict.
3. **Select Regression Model:** Pick from five regression models.
4. **Analyze Results:** View performance metrics and interactive visualizations on the dashboard.

## 📊 Example Metrics
- **Mean Absolute Error (MAE)**
- **Mean Squared Error (MSE)**
- **Root Mean Squared Error (RMSE)**
- **R² Score**

## ⚠️ Known Limitations
- All columns, including the target, are standardized before the train/test split, so the scaler sees the test rows (data leakage) and the reported MAE, MSE and RMSE are in standardized units, not the original units of the target.
- Categorical columns are label encoded, which implies an order that may not exist.
- Outlier removal drops any row with a z-score above 3 in any numeric column, which can remove a lot of data on small datasets.
- Models use default settings and a single 80/20 split.

## 🔮 Future Enhancements
- Integration of Polynomial and Logistic Regression models.
- Customizable reporting and result exports.
- Automated hyperparameter tuning for optimized performance.

## 📄 License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.

## 🙌 Acknowledgements
Created by **Jean-Emmanuel Kouadio**  
© 2024 RegressLy

