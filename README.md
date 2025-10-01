# Applied Data Science Capstone: SpaceX Falcon 9 Landing Prediction

![SpaceX Project Banner](https://placehold.co/1200x400/000000/FFFFFF?text=SpaceX+Landing+Prediction)

## 📜 Project Overview

This project is the capstone for the IBM Data Science Professional Certificate. The primary objective is to build a machine learning model that can predict whether the first stage of a SpaceX Falcon 9 rocket will land successfully. A successful landing is a key factor in reducing the cost of space travel, making this a significant real-world problem.

The project encompasses the entire data science lifecycle, from data collection and wrangling to model training, evaluation, and hyperparameter tuning.

---

##  workflow Project Workflow

The project was broken down into several key stages:

### 1. Data Collection
- **SpaceX API:** Gathered historical launch data, including rocket details, launch sites, payloads, and landing outcomes using the SpaceX REST API.
- **Web Scraping:** Scraped additional data from Wikipedia to supplement the API information, such as booster versions and launch site coordinates.

### 2. Data Wrangling & Preprocessing
- Cleaned and structured the collected data, handling missing values and ensuring data consistency.
- Performed feature engineering to create new variables relevant to the prediction task.
- Applied one-hot encoding to convert categorical variables into a numerical format suitable for machine learning models.
- Utilized **`StandardScaler`** to standardize features, ensuring all variables contribute equally to the model's performance.

### 3. Exploratory Data Analysis (EDA) & Dashboard Visualization
- Performed EDA to understand the relationships between different launch variables and the landing outcome.
- Created an interactive **Dashboard** using Plotly Dash to visualize key metrics, such as success rates by launch site and orbit type.

![Dashboard Screenshot](https://github.com/zeeshanmurad65/Applied-Data-Science-Capstone/blob/main/dashboard.png)

### 4. Model Development & Evaluation
- The dataset was split into training and testing sets using **`train_test_split`** to ensure a fair evaluation of the models.
- Several classification algorithms were trained and evaluated to find the best-performing model:
  - **Logistic Regression**
  - **Support Vector Machine (SVM)**
  - **Decision Tree**
  - **Random Forest**
- The performance of each model was compared based on metrics such as accuracy, precision, recall, and the F1-score.

### 5. Hyperparameter Tuning
- To optimize the best-performing model, **Grid Search Cross-Validation (`GridSearchCV`)** was employed.
- This technique systematically tested a wide range of hyperparameters to find the optimal combination that yielded the highest prediction accuracy.

---

## 🛠️ Technologies & Tools Used
- **Python:** Core programming language.
- **Pandas & NumPy:** For data manipulation and numerical computation.
- **Scikit-learn:** For building and evaluating machine learning models (`LogisticRegression`, `SVC`, `DecisionTreeClassifier`, `RandomForestClassifier`, `GridSearchCV`, `StandardScaler`, `train_test_split`).
- **Matplotlib & Seaborn:** For static data visualizations during EDA.
- **Plotly:** For creating interactive charts and the dashboard.
- **Jupyter Notebook:** For developing and documenting the analysis.

---

## 🚀 How to Run This Project
To replicate this analysis, follow these steps:

```bash
# 1. Clone the repository
git clone [https://github.com/zeeshanmurad/Applied-Data-Science-Capstone.git](https://github.com/your-username/Applied-Data-Science-Capstone.git)

# 2. Navigate to the project directory
cd Applied-Data-Science-Capstone

# 3. Install the required dependencies
pip install -r requirements.txt

# 4. Open and run the Jupyter Notebooks
jupyter notebook
