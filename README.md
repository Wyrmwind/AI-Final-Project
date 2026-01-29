# Movie Industry Trends Analysis - AI Project

## 📊 Project Overview
This project explores trends in the movie industry using data science and machine learning techniques. We analyze a comprehensive dataset of approximately 1 million movie records to uncover insights about production trends, financial performance, genre popularity, and audience ratings over several decades.

## 🎯 Key Objectives
- Investigate temporal changes in movie production from 1950-2025
- Analyze relationships between budget, revenue, and Return on Investment (ROI)
- Explore genre popularity and profitability patterns
- Identify directors with strong critical and commercial performance
- Predict movie success categories (Hit/Average/Flop) using machine learning

## 🔧 Technologies Used
- **Programming Language**: Python 3.x
- **Data Processing**: Pandas, NumPy
- **Machine Learning**: Scikit-learn (Random Forest, Decision Trees, GridSearchCV)
- **Visualization**: Matplotlib, Seaborn
- **Methodologies**: Exploratory Data Analysis (EDA), Feature Engineering, Hyperparameter Tuning

## 📁 Project Structure
```
movie-industry-analysis/
│
├── data/                    # Dataset files
│   ├── raw/                # Original dataset
│   └── processed/          # Cleaned and processed data
│
├── notebooks/              # Jupyter notebooks for analysis
│   ├── 01_eda.ipynb       # Exploratory Data Analysis
│   ├── 02_preprocessing.ipynb  # Data cleaning
│   └── 03_modeling.ipynb  # Machine learning models
│
├── src/                    # Source code
│   ├── data_processing.py # Data cleaning functions
│   ├── visualization.py   # Plotting functions
│   └── models.py          # ML model implementations
│
├── results/               # Generated outputs
│   ├── figures/          # Visualizations and plots
│   └── models/           # Trained model files
│
├── requirements.txt       # Python dependencies
└── README.md             # Project documentation
```

## 📈 Key Findings
- **Production Growth**: Movie production increased nearly tenfold from ~2,500 films (1950) to ~24,000 films (2025)
- **Rating Stability**: Average IMDb rating remained remarkably stable at ~6.49 across decades
- **Budget-Revenue Correlation**: Strong positive correlation (0.895) between budget and revenue
- **ROI Insight**: No correlation between budget and ROI, indicating budget efficiency is independent of spending scale
- **Genre Trends**: Drama dominates production volume, but profitability is distributed across genres

## 🚀 Getting Started

### Prerequisites
- Python 3.8+
- pip package manager

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/movie-industry-analysis.git
   cd movie-industry-analysis
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Download the dataset from Kaggle and place it in the `data/raw/` directory.

### Running the Analysis
1. Start with exploratory data analysis:
   ```bash
   jupyter notebook notebooks/01_eda.ipynb
   ```

2. Run the preprocessing pipeline:
   ```python
   from src.data_processing import clean_dataset
   cleaned_data = clean_dataset('data/raw/movies.csv')
   ```

3. Train the classification model:
   ```python
   from src.models import train_classifier
   model, results = train_classifier(cleaned_data)
   ```

## 📊 Model Performance
The Random Forest classifier was optimized using GridSearchCV for hyperparameter tuning. The model categorizes movies into:
- **Hit**: High commercial success
- **Average**: Moderate performance
- **Flop**: Commercial failure

Key features for prediction include budget, genre, director track record, and IMDb ratings.

## 👥 Contributors
- **Fatima AL Hashedi** - Visualization & Reporting
- **Htet Myet Ko** - Data Analysis & Methodology
- **Aye Nyein Han** - Machine Learning Models

## 📚 References
This project builds upon research in entertainment economics, statistical learning, and big data analytics. Key references include works by Vogel, De Vany, Eliashberg, and contemporary machine learning literature.

## 🔮 Future Enhancements
- Integration of sentiment analysis from social media data
- Incorporation of streaming platform metrics
- Real-time prediction capabilities
- Expanded feature set including screenplay analysis and cultural factors

## 📄 License
This project is for academic purposes as part of the Big Data Analytics and Management program at Bahçeşehir University.

---

*For detailed methodology, results, and analysis, please refer to the full project documentation.*
