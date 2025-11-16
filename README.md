# AI Demand Forecasting Dashboard

An advanced, interactive web-based dashboard for demand forecasting and business analytics powered by machine learning and AI insights.

## Overview

This Jupyter notebook creates a professional Streamlit dashboard that provides comprehensive demand forecasting capabilities with AI-powered insights, anomaly detection, and advanced analytics features. The dashboard uses XGBoost machine learning algorithm for accurate predictions and offers a clean, intuitive interface for data analysis.

## Key Features

### 🤖 AI-Powered Insights
- Automatic trend analysis and pattern recognition
- Data-driven performance recommendations
- Intelligent suggestions based on your data

### 📊 Period Comparison Analysis
- Current vs. previous period comparisons
- Percentage change calculations
- Visual indicators for performance trends
- Side-by-side metric comparisons

### 🔍 Anomaly Detection
- Statistical outlier identification
- Unusual pattern detection
- Automatic flagging of data anomalies
- Visual highlighting of outliers

### 🎯 Machine Learning Forecasting
- XGBoost-based predictive modeling
- Automatic feature engineering
- Model performance metrics (R² score, MAE)
- Confidence in predictions

### 📈 Interactive Visualizations
- Revenue trends over time
- Forecast vs. actual comparisons
- Category-wise performance breakdowns
- Regional and segment analysis
- Anomaly highlighting

### 💾 Multi-Format Export
- CSV file export
- Excel workbooks with multiple sheets
- Text-based reports
- Downloadable forecasts and insights

### 🎨 Professional UI
- Clean, modern interface
- Responsive design
- Interactive filters and controls
- Real-time data updates

## Requirements

### Software Dependencies
- Python 3.7+
- Jupyter Notebook or Google Colab
- ngrok account (free tier works)

### Python Packages
All packages are automatically installed by the notebook:
- `streamlit` - Web dashboard framework
- `plotly` - Interactive visualizations
- `scikit-learn` - Machine learning utilities
- `xgboost` - Gradient boosting algorithm
- `pandas` - Data manipulation
- `numpy` - Numerical computing
- `pyngrok` - ngrok integration
- `openpyxl` - Excel file handling

## Setup and Installation

### Step 1: Get ngrok Token
1. Visit [ngrok.com](https://dashboard.ngrok.com/get-started/your-authtoken)
2. Sign up for a free account
3. Copy your authentication token

### Step 2: Run the Notebook
1. Open `Dashboard.ipynb` in Google Colab or Jupyter Notebook
2. Run the single code cell
3. When prompted, enter your ngrok authentication token
4. Wait for installation and setup to complete

### Step 3: Access the Dashboard
1. The notebook will output a public URL (e.g., `https://xxxx.ngrok-free.app`)
2. Click or copy the URL to access your dashboard
3. Keep the notebook running while using the dashboard

## Data Format Requirements

### Required Columns
Your CSV file must include:
- **Order_Date**: Date column (various formats accepted)
- **Revenue**: Numerical revenue/demand values

### Optional Columns
These columns enable additional features:
- **Product_Category**: Product categories for segmentation
- **Region**: Geographic regions for regional analysis
- **Customer_Segment**: Customer segments for targeted insights

### Example CSV Structure
```csv
Order_Date,Revenue,Product_Category,Region,Customer_Segment
2024-01-01,1500,Electronics,North,Enterprise
2024-01-02,2300,Furniture,South,SMB
2024-01-03,1800,Office,East,Enterprise
```

## How to Use

### 1. Upload Data
- Click "Browse files" or drag and drop your CSV file
- The dashboard automatically processes and validates your data

### 2. Configure Settings (Sidebar)
- **Forecast Horizon**: Choose 7, 14, 30, or 90 days
- **Filters**: Select specific categories, regions, or segments
- **Date Range**: Filter data by custom date ranges

### 3. Explore Insights
- **AI Insights Section**: View automatic trend analysis and recommendations
- **Period Comparison**: See how current performance compares to previous periods
- **Key Metrics**: Monitor total revenue, average daily revenue, and trends

### 4. Analyze Forecasts
- Review the forecast chart showing predicted demand
- Check model performance metrics
- Examine confidence levels in predictions

### 5. Detect Anomalies
- View highlighted anomalies in the data
- Understand unusual patterns or outliers
- Use insights to investigate data quality issues

### 6. Export Results
- Choose your preferred format (CSV, Excel, or TXT)
- Download forecasts, insights, and detailed reports
- Share findings with stakeholders

## Features in Detail

### AI Insights Engine
The dashboard analyzes your data and provides:
- Trend direction and strength
- Performance assessment
- Actionable recommendations
- Data quality observations

### Forecasting Model
- Uses XGBoost gradient boosting algorithm
- Automatic date feature engineering (day, month, year, day of week)
- Category encoding for segmentation
- Train-test split validation
- Performance metrics reporting

### Anomaly Detection
- Statistical Z-score based detection
- Configurable sensitivity (default: 2 standard deviations)
- Visual markers on charts
- Detailed anomaly reports

### Export Options

#### CSV Export
- Clean, structured data
- Forecast predictions
- Easy to import into other tools

#### Excel Export
Multiple sheets including:
- Forecasts
- Insights summary
- Anomaly details
- Model metrics
- Data statistics

#### Text Report
- Human-readable format
- Executive summary
- Key findings
- Detailed insights

## Technical Architecture

### Frontend
- **Streamlit**: Web application framework
- **Plotly**: Interactive chart library
- **Custom CSS**: Professional styling

### Backend
- **XGBoost**: Machine learning forecasting
- **Pandas**: Data processing and manipulation
- **NumPy**: Numerical computations
- **Scikit-learn**: ML utilities and preprocessing

### Deployment
- **ngrok**: Secure tunneling service
- **Google Colab**: Cloud-based execution environment

## Troubleshooting

### Dashboard doesn't load
- Ensure ngrok token is correctly entered
- Check that the notebook cell is still running
- Try refreshing the ngrok URL

### Data upload fails
- Verify CSV file has required columns (Order_Date, Revenue)
- Check date format is recognizable
- Ensure file size is reasonable (<100MB)

### Forecasts seem inaccurate
- Ensure sufficient historical data (minimum 30 days recommended)
- Check for data quality issues or missing values
- Try different forecast horizons

### Export not working
- Check browser popup blocker settings
- Try a different export format
- Ensure sufficient data is loaded

## Limitations

- Requires continuous notebook execution
- ngrok free tier has session time limits
- Single user access per notebook instance
- Performance depends on data size and complexity

## Best Practices

1. **Data Quality**: Clean your data before uploading
2. **Historical Data**: Provide at least 2-3 months of history
3. **Regular Updates**: Re-run forecasts with new data periodically
4. **Validate Results**: Cross-check predictions with domain knowledge
5. **Save Exports**: Download insights and forecasts for record-keeping

## Security Note

The ngrok URL is publicly accessible. Do not upload sensitive or confidential data without proper authorization. Consider using ngrok's paid features for password protection if needed.

## Support and Updates

For issues or questions:
- Review the troubleshooting section
- Check data format requirements
- Ensure all dependencies are properly installed

## License

This dashboard is provided as-is for educational and business analytics purposes.

---

**Version**: 1.0  
**Last Updated**: 2025  
**Platform**: Google Colab / Jupyter Notebook  
**Framework**: Streamlit + XGBoost + Plotly
