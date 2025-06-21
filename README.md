# IntelligoProject - E-commerce Product Analysis and Prediction

## 📊 Project Overview

This project performs comprehensive analysis and machine learning predictions on e-commerce product data, specifically focusing on fashion products from Tokopedia. The analysis includes both regression and classification tasks to predict product prices and ratings.

## 🎯 Objectives

1. **Price Prediction**: Predict product prices based on various features using Random Forest Regression
2. **Rating Classification**: Classify products into rating categories (1-5 stars) using Random Forest Classification
3. **Data Analysis**: Explore relationships between product features and their impact on pricing and ratings

## 📁 Dataset

The project uses `final_project.csv` containing e-commerce product data

## 🔧 Technologies Used

- **Python 3.x**
- **pandas**: Data manipulation and analysis
- **numpy**: Numerical computing
- **matplotlib**: Data visualization
- **seaborn**: Statistical data visualization
- **scikit-learn**: Machine learning algorithms
  - Random Forest Regressor
  - Random Forest Classifier
  - StandardScaler
  - LabelEncoder
  - Cross-validation
  - Train-test split

## 📈 Project Workflow

### 1. Data Exploration and Preprocessing
- Load and explore the dataset structure
- Generate descriptive statistics
- Create visualizations (histograms, count plots, correlation heatmaps)
- Handle missing values and duplicates
- Feature selection and engineering

### 2. Data Cleaning
- Remove unnecessary columns (category, city, image_url, etc.)
- Convert data types appropriately
- Apply log transformation for better distribution
- Encode categorical variables using LabelEncoder

### 3. Model Development

#### Price Prediction (Regression)
- **Target**: Product price
- **Features**: gold_merchant, jumlah_review, jumlah_view, quantity_sold, rating
- **Algorithm**: Random Forest Regressor
- **Evaluation**: Cross-validation with R² score and RMSE

#### Rating Classification
- **Target**: Product rating (converted to categorical labels)
- **Features**: gold_merchant, jumlah_review, quantity_sold, subcategory
- **Algorithm**: Random Forest Classifier
- **Evaluation**: Cross-validation and accuracy

### 4. Model Training and Evaluation
- Split data into training and testing sets (80/20)
- Apply StandardScaler for feature normalization
- Train Random Forest models
- Evaluate performance using appropriate metrics

## 🚀 Getting Started

### Prerequisites
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

### Running the Project
1. Clone this repository
2. Ensure `data/final_project.csv` is in the correct directory
3. Open and run `index.ipynb` in Jupyter Notebook or JupyterLab
4. Follow the notebook cells sequentially for complete analysis

## 📁 Project Structure
```
IntelligoProject/
│
├── index.ipynb          # Main analysis notebook
├── README.md           # Project documentation
├── data/
│   └── final_project.csv # Dataset
```

## 🔍 Key Insights

1. **Feature Importance**: Gold merchant status, number of reviews, and product views are significant predictors
2. **Data Distribution**: Log transformation helps normalize skewed price distributions
3. **Model Performance**: Random Forest algorithms show good performance for both regression and classification tasks
4. **Business Value**: Models can help sellers optimize pricing and understand rating patterns

## 📝 Future Improvements

- [ ] Hyperparameter tuning for Random Forest models
- [ ] Feature engineering (creating new meaningful features)
- [ ] Testing other algorithms (XGBoost, Neural Networks)
- [ ] Model deployment and API creation
- [ ] Real-time prediction interface

## 👥 Contributing

Feel free to contribute to this project by:
1. Forking the repository
2. Creating a feature branch
3. Making improvements
4. Submitting a pull request

## 📄 License

This project is open-source and available under the MIT License.

---

For questions or collaborations, please reach out through GitHub issues or contact information provided in the profile.
