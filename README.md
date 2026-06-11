# 🦈 Shark-Attacks-Analysis
This is a data analysis project examining global shark attack incidents based on the publicly available **Global Shark Attack File (GSAF)**. The dataset can be obtained from the following link: https://www.sharkattackfile.net/spreadsheets/GSAF5.xls. This project provides statistical analysis and visualisations of shark attack data which includes:
  1. Annual shark attack patterns and distribution
  2. Attack frequency and fatality rates by country
  3. Which activities put people at the highest risk for a shark attack
  4. Breakdown of fatal vs non-fatal incidents
  5. statistical analysis of attack frequency (skew and kurtosis)

The aim of this project is to understand shark behaviour and human-shark interaction and thus prove that there is a misconception that sharks are man-eating beasts.

## 🔍 Key Findings

### Dataset Overview
- **Time Period**: 2000-2025
- **Total Incidents**: 2,785 shark attack records (after filtering)
- **Fatality Rate**: ~10% of incidents are fatal, 90% non-fatal

### Statistical Insights

**Annual Attack Distribution:**
- **Mean**: ~99.88 attacks per year
- **Median**: 99.5 attacks per year
- **Range**: 50 to 130 attacks per year
- **Skewness**: -0.69 (slight left skew, more years with higher attack counts)
- **Kurtosis**: 0.65 (slightly heavier tails than normal distribution)

### Top Findings

1. **Most Common Activities**:
   - Surfing, Swimming, Diving, and Fishing dominate shark attack incidents

2. **Highest Risk Countries**:
   - USA, Australia, and South Africa lead in both attack frequency and fatality rates

3. **Activity Risk Analysis**:
   - Different water activities have varying fatality rates
   - Swimming and surfing account for the majority of incidents

## 📝 Methodology

### 1. Data Preprocessing
  - Removal of missing values in Year column
  - Filtering for years 2000-2025
  - Exclusion of "Questionable" attack classifications
  - Creation of fatality indicator (Is_Fatal: 1=Fatal, 0=Non-Fatal)

### 2. Descriptive Statistics
  - Annual attack count analysis
  - Mean, median, standard deviation calculations
  - Quartile analysis (Q1, Q2, Q3)

### 3. Temporal Trends
  - Bar chart visualization of global shark attacks per year
  - Year-over-year trend analysis

### 4. Distribution Analysis
  - Histogram with KDE (Kernel Density Estimation)
  - Statistical measures: skewness and kurtosis
  - Mean and median indicators

### 5. Activity Analysis
  - Top 10 most common activities during shark attacks
  - Fatality rate comparison across activities
  - Stacked bar chart showing non-fatal vs. fatal proportions

### 6. Geographical Analysis
  - Fatality rates by country
  - Focus on top 10 most attacked countries
  - Regional risk assessment

## 🛠️ Technologies & Libraries

- **Python 3**: Core programming language
- **Pandas**: Data manipulation and analysis
- **NumPy**: Numerical computations
- **Matplotlib**: Base plotting library
- **Seaborn**: Statistical data visualization
- **SciPy**: Statistical analysis (skew, kurtosis)
- **Plotly**: Interactive charts
- **Google Colab**: Development environment

## 🚀 Getting Started

### Prerequisites
- Google Colab account (or Python environment with required libraries)
- Access to the shark attack dataset

### Running the Analysis

1. Open `shark.ipynb` in Google Colab or in Jupyter Notebook
2. Mount your Google Drive (for Google Colab only):
   ```python
   from google.colab import drive
   drive.mount('/content/drive')
3. Run the cells sequentially

## 📖 Data Dictionary

| Column    | Description                                     |
|-----------|-------------------------------------------------|
| Year      | Year of the incident                            |
| Type      | Classification of attack (Provoked/Unprovoked)  |
| Country   | Country where incident occurred                 |
| State     | State/Province location                         |
| Activity  | Activity being performed during attack          |
| Fatal Y/N | Whether the incident was fatal (Y/N)            |
| Is_Fatal  | Numeric indicator (1=Fatal, 0=Non-Fatal)        |
| Date      | Date of incident                                |

## 👤 Author
pointernullbrain


Last Updated: 2026
Data Coverage: 2000-2025
Total Records Analyzed: 2,785 incidents
