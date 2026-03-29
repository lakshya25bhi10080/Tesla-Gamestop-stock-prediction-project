# Tesla-GameStop-Stock-Prediction-Project


> A comprehensive financial data analysis and visualization project for AIML coursework 
 
**Student Name:** Lakshya Pareek

**Registration Number** 25BHI10080

**Institution:** VIT Bhopal

---

## 🎯 Project Objective

To develop a comprehensive stock analysis and Prediction system that:
- **Fetches real-time stock data** from Yahoo Finance API
- **Scrapes financial data** from web sources using BeautifulSoup
- **Processes and cleans data** using Pandas
- **Performs statistical analysis** on Tesla (TSLA) and GameStop (GME) stocks
- **Generates interactive visualizations** using Plotly and Matplotlib
- **Provides comparative analysis** and correlation insights

---

## 📋 Table of Contents

1. [Project Overview](#-project-overview)
2. [Features](#-features)
3. [Technology Stack](#-technology-stack)
4. [Installation](#-installation)
5. [Project Structure](#-project-structure)
6. [Usage Guide](#-usage-guide)
7. [Algorithm & Pseudocode](#-algorithm--pseudocode)
8. [System Architecture](#-system-architecture)
9. [Data Flow Diagram](#-data-flow-diagram)
10. [Key Functions & Modules](#-key-functions--modules)
11. [Results & Analysis](#-results--analysis)
12. [Project Screenshots](#-Project-sceenshot)
13. [Learning Outcomes](#-learning-outcomes)
14. [Future Enhancements](#-future-enhancements)
15. [Contributors](#-contributors)
16. [Acknowledgments](#-acknowledgments)

---

## 🎨 Project Overview

### What is This Project?

This project is a **full-stack financial data analysis application** that demonstrates:
- **Data Collection:** API integration and web scraping
- **Data Processing:** Pandas-based data cleaning and transformation
- **Data Analysis:** Statistical calculations and insights
- **Data Visualization:** Interactive and static visualizations
- **Problem Solving:** Fixing real-world data issues

### Why This Project?

✅ Demonstrates real-world data science skills  
✅ Shows API integration and web scraping proficiency  
✅ Illustrates data manipulation and analysis techniques  
✅ Creates professional visualizations  
✅ Solves authentic problems with financial data  

---
# 💻 Tech Stack:
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) 
![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white) 
![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)
![Jupyter](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-%233F4F75.svg?style=for-the-badge&logo=plotly&logoColor=white)
![BeautifulSoup](https://img.shields.io/badge/BeautifulSoup4-green?style=for-the-badge)

---

## 🌟 Features

### Core Features:
- ✅ **Real-time Data Fetching** - Downloads latest stock data from Yahoo Finance
- ✅ **Web Scraping** - Extracts revenue data from HTML tables
- ✅ **Data Cleaning** - Handles missing values and data type conversions
- ✅ **Statistical Analysis** - Calculates mean, median, std dev, volatility
- ✅ **Interactive Plots** - Plotly-based interactive visualizations
- ✅ **Static Dashboards** - Matplotlib-based multi-panel analysis
- ✅ **Comparative Analysis** - Tesla vs GameStop performance comparison
- ✅ **Correlation Analysis** - Price correlation between stocks
- ✅ **Error Handling** - Robust exception handling with fallbacks

### Advanced Features:
- 📈 Moving averages (30-day & 90-day)
- 📊 Daily returns distribution
- 📉 Volatility tracking
- 🔄 Data normalization for comparison
- 💾 CSV export functionality
- 📝 Comprehensive logging

---

## 🔧 Technology Stack

| Technology | Purpose | Version |
|-----------|---------|---------|
| **Python** | Core programming language | 3.7+ |
| **Pandas** | Data manipulation & analysis | Latest |
| **yfinance** | Yahoo Finance data fetching | Latest |
| **BeautifulSoup4** | Web scraping | Latest |
| **Plotly** | Interactive visualizations | Latest |
| **Matplotlib** | Static visualizations | Latest |
| **Seaborn** | Statistical visualizations | Latest |
| **NumPy** | Numerical computations | Latest |
| **Jupyter** | Interactive notebooks | Latest |
| **Requests** | HTTP requests | Latest |

---

## 📦 Installation

### Prerequisites:
- Python 3.7 or higher
- pip package manager
- Internet connection (for data fetching)

### Step 1: Clone/Download Project
```bash
# Navigate to project directory
cd Tesla-Stock-Analysis
```

### Step 2: Install Dependencies
```bash
# Install all required packages
pip install yfinance pandas requests beautifulsoup4 plotly matplotlib seaborn numpy jupyter

# Or use requirements file (if provided):
pip install -r requirements.txt
```

### Step 3: Verify Installation
```bash
# Test Python
python --version

# Test packages
python -c "import pandas, yfinance, plotly; print('✓ All packages installed!')"
```

### Step 4: Run the Project

**Option A - Jupyter Notebook:**
```bash
jupyter notebook Tesla_Stock_Analysis_Complete.ipynb
# Then click Cell → Run All
```

**Option B - Python Script:**
```bash
python complete_codebase.py
```

---

## 📁 Project Structure

```
Tesla-Stock-Analysis/
│
├── 📄 README.md                           # Project documentation (this file)
├── 📄 DOCUMENTATION.md                    # Detailed technical documentation
├── 📄 requirements.txt                    # Python dependencies
│
├── 📓 Jupyter Notebooks/
│   ├── Tesla_Stock_Analysis_Complete.ipynb   # Main analysis notebook
│   └── Tesla_Stock_Analysis_Complete_FIXED.ipynb (Fixed version)
│
├── 🐍 Python Scripts/
│   ├── complete_codebase.py               # Complete corrected codebase
│   ├── tesla_stock_analysis_corrected.py  # Cleaned version
│   └── fix_notebook.py                    # Automated bug fixer
│
├── 📚 Documentation Files/
│   ├── QUICKSTART.md                      # Quick start guide
│   ├── JUPYTER_GUIDE.md                   # Jupyter notebook guide
│   ├── SYNTAX_ERROR_FIX.md                # Bug fix documentation
│   ├── README.md                          # Issues report
│   └── issues_summary.csv                 # Bug reference table
│
├── 📊 Data Files/ (Generated during runtime)
│   ├── tesla_stock_data.csv
│   ├── tesla_revenue_data.csv
│   ├── gme_stock_data.csv
│   └── gme_revenue_data.csv
│
└── 📈 Output Files/ (Generated after analysis)
    ├── tesla_plot.png
    ├── gme_plot.png
    ├── comparative_analysis.png
    └── correlation_analysis.png
```

---

## 🚀 Usage Guide

### Basic Usage:

```python
# 1. Import necessary libraries
import yfinance as yf
import pandas as pd
from bs4 import BeautifulSoup
import requests

# 2. Fetch stock data
tesla = yf.Ticker("TSLA")
tesla_data = tesla.history(period="max")

# 3. View data
print(tesla_data.head())
print(tesla_data.describe())

# 4. Scrape revenue data
url = "https://example.com/revenue"
html = requests.get(url).text
soup = BeautifulSoup(html, "html.parser")

# 5. Create visualizations
import matplotlib.pyplot as plt
plt.plot(tesla_data['Close'])
plt.show()
```

### Advanced Usage:

See the complete codebase for advanced examples including:
- Custom indicator calculations
- Portfolio analysis
- Multi-stock comparison
- Automated reporting

---

## 🧠 Algorithm & Pseudocode

### Main Algorithm - Stock Analysis Pipeline

```
ALGORITHM StockAnalysisPipeline(stock_ticker_list, date_range)

INPUT: 
    - stock_ticker_list: Array of stock symbols (e.g., ["TSLA", "GME"])
    - date_range: Time period for analysis
    
OUTPUT:
    - Analysis reports, visualizations, statistics

BEGIN
    // Phase 1: Data Collection
    FOR EACH ticker IN stock_ticker_list DO
        PRINT "Fetching data for ", ticker
        stock_data[ticker] ← FetchYahooFinanceData(ticker, date_range)
        revenue_data[ticker] ← ScrapeRevenueData(ticker)
        PRINT "✓ Data loaded successfully"
    END FOR
    
    // Phase 2: Data Cleaning
    FOR EACH ticker IN stock_ticker_list DO
        PRINT "Cleaning data for ", ticker
        stock_data[ticker] ← RemoveMissingValues(stock_data[ticker])
        revenue_data[ticker] ← ConvertDataTypes(revenue_data[ticker])
        stock_data[ticker] ← NormalizeData(stock_data[ticker])
    END FOR
    
    // Phase 3: Statistical Analysis
    FOR EACH ticker IN stock_ticker_list DO
        PRINT "Calculating statistics for ", ticker
        stats[ticker] ← CalculateStatistics(stock_data[ticker])
            - mean_price ← Mean(stock_data[ticker].Close)
            - std_price ← StandardDeviation(stock_data[ticker].Close)
            - volatility ← CalculateVolatility(stock_data[ticker])
            - daily_returns ← CalculateDailyReturns(stock_data[ticker])
        PRINT stats[ticker]
    END FOR
    
    // Phase 4: Visualization
    FOR EACH ticker IN stock_ticker_list DO
        PRINT "Creating visualizations for ", ticker
        
        // Create interactive plot
        interactive_plot[ticker] ← CreatePlotlyVisualization(
            stock_data[ticker],
            revenue_data[ticker],
            ticker
        )
        
        // Create dashboard
        dashboard[ticker] ← CreateMatplotlibDashboard(
            stock_data[ticker],
            ticker
        )
    END FOR
    
    // Phase 5: Comparative Analysis
    PRINT "Creating comparative analysis"
    comparison ← CompareStocks(stock_ticker_list, stock_data)
        - normalized_prices ← NormalizeAllPrices()
        - volatility_comparison ← CompareVolatility()
        - correlation ← CalculateCorrelation()
    
    // Phase 6: Generate Reports
    PRINT "Generating reports"
    GenerateStatisticalReport(stats)
    GenerateComparisonReport(comparison)
    
    PRINT "Analysis complete! ✓"
END
```

### Key Sub-Algorithms:

#### Data Fetching Algorithm:
```
ALGORITHM FetchYahooFinanceData(ticker, period)
BEGIN
    TRY
        connection ← Connect to Yahoo Finance API
        data ← Download(ticker, period="max")
        RETURN data with columns [Date, Open, High, Low, Close, Volume]
    CATCH exception
        PRINT "Error fetching data: ", exception
        RETURN dummy_data
    END TRY
END
```

#### Data Cleaning Algorithm:
```
ALGORITHM CleanData(raw_data)
BEGIN
    // Remove duplicates
    cleaned_data ← RemoveDuplicates(raw_data)
    
    // Handle missing values
    FOR EACH row IN cleaned_data DO
        IF row contains NULL THEN
            cleaned_data ← InterpolateOrRemove(row)
        END IF
    END FOR
    
    // Convert data types
    cleaned_data.Close ← ConvertToFloat(cleaned_data.Close)
    cleaned_data.Volume ← ConvertToInteger(cleaned_data.Volume)
    cleaned_data.Date ← ConvertToDateTime(cleaned_data.Date)
    
    // Remove outliers (optional)
    cleaned_data ← RemoveOutliers(cleaned_data)
    
    RETURN cleaned_data
END
```

#### Statistical Analysis Algorithm:
```
ALGORITHM CalculateStatistics(stock_data)
BEGIN
    statistics ← EMPTY_DICT
    
    statistics["count"] ← LENGTH(stock_data)
    statistics["mean"] ← SUM(stock_data.Close) / COUNT
    statistics["median"] ← MEDIAN(stock_data.Close)
    statistics["std"] ← STANDARD_DEVIATION(stock_data.Close)
    statistics["min"] ← MIN(stock_data.Close)
    statistics["max"] ← MAX(stock_data.Close)
    
    // Calculate returns
    returns ← []
    FOR i FROM 1 TO LENGTH(stock_data)-1 DO
        daily_return ← (Close[i] - Close[i-1]) / Close[i-1] * 100
        returns.APPEND(daily_return)
    END FOR
    
    statistics["mean_return"] ← MEAN(returns)
    statistics["volatility"] ← STDEV(returns)
    
    RETURN statistics
END
```

---

## 🏗️ System Architecture

### High-Level Architecture Diagram:

```
┌─────────────────────────────────────────────────────────────┐
│                    USER INTERFACE LAYER                      │
│         (Jupyter Notebook / Python Console)                  │
└────────────────────────┬────────────────────────────────────┘
                         │
┌────────────────────────▼────────────────────────────────────┐
│                    APPLICATION LAYER                         │
│  ┌──────────────┐  ┌──────────────┐  ┌──────────────┐       │
│  │   Data       │  │  Analysis    │  │ Visualization│       │
│  │  Fetching    │  │  Module      │  │   Module     │       │
│  │  Module      │  │              │  │              │       │
│  └──────────────┘  └──────────────┘  └──────────────┘       │
└────────────────────────┬────────────────────────────────────┘
                         │
┌────────────────────────▼────────────────────────────────────┐
│                    DATA LAYER                                │
│  ┌──────────────┐  ┌──────────────┐  ┌──────────────┐       │
│  │   Pandas     │  │   NumPy      │  │   Raw Data   │       │
│  │  DataFrames  │  │   Arrays     │  │   Cache      │       │
│  └──────────────┘  └──────────────┘  └──────────────┘       │
└────────────────────────┬────────────────────────────────────┘
                         │
┌────────────────────────▼────────────────────────────────────┐
│                   EXTERNAL SOURCES                           │
│  ┌──────────────┐  ┌──────────────┐  ┌──────────────┐       │
│  │   Yahoo      │  │   Web        │  │   CSV Files  │       │
│  │   Finance    │  │   Scraping   │  │              │       │
│  └──────────────┘  └──────────────┘  └──────────────┘       │
└──────────────────────────────────────────────────────────────┘
```

---

## 📊 Data Flow Diagram

```
START
  │
  ├─→ [1] FETCH DATA
  │   │
  │   ├─→ Yahoo Finance API (yfinance)
  │   │   └─→ Stock prices (Open, High, Low, Close, Volume)
  │   │
  │   └─→ Web Scraping (BeautifulSoup)
  │       └─→ Revenue data from HTML tables
  │
  ├─→ [2] DATA CLEANING
  │   │
  │   ├─→ Remove missing values
  │   ├─→ Convert data types
  │   ├─→ Handle duplicates
  │   └─→ Normalize data
  │
  ├─→ [3] DATA ANALYSIS
  │   │
  │   ├─→ Calculate statistics
  │   │   ├─→ Mean, Median, Std Dev
  │   │   ├─→ Min, Max
  │   │   └─→ Volatility, Returns
  │   │
  │   ├─→ Calculate indicators
  │   │   ├─→ Moving averages (30, 90)
  │   │   ├─→ Daily returns
  │   │   └─→ Volatility
  │   │
  │   └─→ Comparative analysis
  │       ├─→ Normalize prices
  │       ├─→ Compare volatility
  │       └─→ Calculate correlation
  │
  ├─→ [4] VISUALIZATION
  │   │
  │   ├─→ Interactive Plots (Plotly)
  │   │   ├─→ Stock price + Revenue
  │   │   └─→ Correlation scatter
  │   │
  │   └─→ Static Dashboards (Matplotlib)
  │       ├─→ Price trends
  │       ├─→ Volume analysis
  │       ├─→ Returns distribution
  │       └─→ Moving averages
  │
  ├─→ [5] GENERATE REPORTS
  │   │
  │   ├─→ Statistical summaries
  │   ├─→ Comparative analysis
  │   └─→ Insights & trends
  │
  └─→ [6] OUTPUT
      │
      ├─→ Console output
      ├─→ Visualizations
      ├─→ CSV exports
      └─→ Reports

END
```

---

## 🔧 Key Functions & Modules

### 1. **Data Fetching Module**

```python
def fetch_stock_data(ticker, period="max"):
    """
    Fetch stock data from Yahoo Finance
    
    Args:
        ticker (str): Stock symbol (e.g., "TSLA")
        period (str): Time period for data
        
    Returns:
        pd.DataFrame: Stock data with OHLCV columns
    """
```

### 2. **Web Scraping Module**

```python
def scrape_revenue_data(url, table_index):
    """
    Scrape revenue data from HTML tables
    
    Args:
        url (str): URL to scrape
        table_index (int): Index of table to extract
        
    Returns:
        pd.DataFrame: Revenue data with Date and Revenue columns
    """
```

### 3. **Data Cleaning Module**

```python
def clean_data(raw_data):
    """
    Clean and prepare data for analysis
    
    Args:
        raw_data (pd.DataFrame): Raw data with potential issues
        
    Returns:
        pd.DataFrame: Cleaned data ready for analysis
    """
```

### 4. **Statistical Analysis Module**

```python
def calculate_statistics(stock_data):
    """
    Calculate key statistics for stock data
    
    Args:
        stock_data (pd.DataFrame): Stock data
        
    Returns:
        dict: Dictionary containing all statistics
    """
```

### 5. **Visualization Module**

```python
def create_interactive_plot(stock_data, revenue_data, stock_name):
    """
    Create interactive Plotly visualization
    
    Args:
        stock_data (pd.DataFrame): Stock price data
        revenue_data (pd.DataFrame): Revenue data
        stock_name (str): Name for title
        
    Returns:
        plotly.graph_objects.Figure: Interactive figure
    """

def create_dashboard(stock_data, stock_name):
    """
    Create matplotlib analysis dashboard
    
    Args:
        stock_data (pd.DataFrame): Stock data
        stock_name (str): Name for titles
    """
```

---

## 📈 Results & Analysis

### Analysis Output:

The project generates comprehensive analysis including:

1. **Statistical Reports**
   - Price statistics (mean, median, std dev)
   - Volatility measurements
   - Daily returns analysis
   - Trading volume metrics

2. **Visual Reports**
   - 6 professional charts
   - Interactive Plotly visualizations
   - Multi-panel Matplotlib dashboards
   - Comparative analysis plots

3. **Data Insights**
   - Stock performance trends
   - Price correlation analysis
   - Volatility patterns
   - Volume trends

### Expected Results:

- ✅ Tesla data: ~3,859 historical records
- ✅ Tesla revenue: ~45 quarterly records
- ✅ GameStop data: ~4,892 historical records
- ✅ GameStop revenue: ~28 quarterly records
- ✅ Execution time: ~70 seconds (first run)

---
## Project Screenshot
![Screenshot1](https://github.com/shamiquekhan/Tesla-GameStop-Stock-Analysis-Project/blob/main/Screenshots/Screenshot%202025-11-22%20193042.png)
![Screenshot2](https://github.com/shamiquekhan/Tesla-GameStop-Stock-Analysis-Project/blob/main/Screenshots/Screenshot%202025-11-22%20193056.png)
![Screenshot3](https://github.com/shamiquekhan/Tesla-GameStop-Stock-Analysis-Project/blob/main/Screenshots/Screenshot%202025-11-22%20193112.png)
![Screenshot4](https://github.com/shamiquekhan/Tesla-GameStop-Stock-Analysis-Project/blob/main/Screenshots/Screenshot%202025-11-22%20195233.png)
![Screenshot5](https://github.com/shamiquekhan/Tesla-GameStop-Stock-Analysis-Project/blob/main/Screenshots/Screenshot%202025-11-22%20195242.png)
![Screenshot7](https://github.com/shamiquekhan/Tesla-GameStop-Stock-Analysis-Project/blob/main/Screenshots/Screenshot%202025-11-22%20195257.png)
![Screenshot8](https://github.com/shamiquekhan/Tesla-GameStop-Stock-Analysis-Project/blob/main/Screenshots/Screenshot%202025-11-22%20195316.png)
![Screenshot9](https://github.com/shamiquekhan/Tesla-GameStop-Stock-Analysis-Project/blob/main/Screenshots/Screenshot%202025-11-22%20212802.png)
![Screenshot10](https://github.com/shamiquekhan/Tesla-GameStop-Stock-Analysis-Project/blob/main/Screenshots/Screenshot%202025-11-22%20212846.png)
![Screenshot11](https://github.com/shamiquekhan/Tesla-GameStop-Stock-Analysis-Project/blob/main/Screenshots/Screenshot%202025-11-22%20212916.png)  
---
## 🎓 Learning Outcomes

This project demonstrates understanding of:

### 1. **Data Collection & APIs**
- ✅ Working with RESTful APIs (Yahoo Finance)
- ✅ HTTP requests and responses
- ✅ JSON/CSV data formats

### 2. **Web Scraping**
- ✅ HTML parsing with BeautifulSoup
- ✅ Table extraction
- ✅ Data validation

### 3. **Data Processing**
- ✅ Pandas DataFrames manipulation
- ✅ Data cleaning techniques
- ✅ Type conversions
- ✅ Missing value handling

### 4. **Statistical Analysis**
- ✅ Descriptive statistics
- ✅ Correlation analysis
- ✅ Volatility calculations
- ✅ Moving averages

### 5. **Data Visualization**
- ✅ Interactive plots (Plotly)
- ✅ Static visualizations (Matplotlib)
- ✅ Multi-panel dashboards
- ✅ Professional formatting

### 6. **Software Engineering**
- ✅ Error handling
- ✅ Code organization
- ✅ Documentation
- ✅ Testing practices

---

## 🚀 Future Enhancements

### Potential Improvements:

1. **Advanced Analytics**
   - Technical indicators (RSI, MACD, Bollinger Bands)
   - Predictive models (LSTM, ARIMA)
   - Machine learning classification

2. **Portfolio Management**
   - Multi-stock analysis
   - Portfolio optimization
   - Risk assessment

3. **Real-time Features**
   - Live data updates
   - Email notifications
   - Automated alerts

4. **User Interface**
   - Web dashboard (Flask/Django)
   - Mobile app
   - API endpoint

5. **Data Storage**
   - Database integration (SQL/NoSQL)
   - Time-series database
   - Cloud storage

6. **Reporting**
   - PDF report generation
   - Email integration
   - Scheduled reports

---

## 👨‍💻 Contributors

- **Lakshya Pareek** - Developer & Student
  - VIT Bhopal
  - CSE Student
  - AI & ML Enthusiast

---

## 🙏 Acknowledgments

Special thanks to:
- **VIT Bhopal** for providing resources and support
- **Open-source community** for excellent libraries:
  - pandas, yfinance, BeautifulSoup, Plotly, Matplotlib
- **Tech documentation** from all referenced sources

---

## 📄 License

This project is created for educational purposes as part of AIML coursework.

---

## 📚 References

1. **yfinance Documentation:** https://github.com/ranaroussi/yfinance
2. **Pandas Documentation:** https://pandas.pydata.org/
3. **Plotly Documentation:** https://plotly.com/python/
4. **BeautifulSoup Documentation:** https://www.crummy.com/software/BeautifulSoup/
5. **Matplotlib Documentation:** https://matplotlib.org/
6. **Financial Data Analysis:** https://www.investopedia.com/

---

## 📋 Checklist for Submission

- ✅ Complete source code
- ✅ Jupyter notebook with analysis
- ✅ Comprehensive documentation
- ✅ Pseudocode and algorithms
- ✅ System architecture
- ✅ Bug fixes and improvements
- ✅ Learning outcomes
- ✅ Future enhancements
- ✅ Professional README

---

<div align="center">


*"Data tells stories. Let's read them together."*

---

</div>
