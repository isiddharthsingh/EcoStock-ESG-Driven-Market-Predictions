# EcoStock-ESG-Driven-Market-Predictions

## Project Overview
This project focuses on developing predictive models for stock prices using Environmental, Social, and Governance (ESG) factors as key inputs. By integrating sustainability metrics with financial performance, the project employs various advanced statistical and econometric models to forecast stock prices.

## Project Description
### Objectives
- To predict stock prices using ESG sentiment analysis derived from news data.
- To compare the effectiveness of different time series models in stock price prediction.

### Models Implemented
1. **Autoregressive Integrated Moving Average (ARIMA)**
2. **Simple Moving Average (SMA)**
3. **Exponential Smoothing**
4. **Seasonal ARIMA with eXogenous variables (SARIMAX)**
5. **Vector Autoregression Moving-Average with eXogenous variables (VARMAX)**
6. **Ordinary Least Squares (OLS)**

## Data Sources
- **Stock Data:** Retrieved from the Alpha Vantage API.
- **News Sentiment Data:** Collected using the Alpha Vantage News Sentiment API.

## Methodology
1. **Data Collection:**
   - **Stock Data:** Queried from Alpha Vantage API for META Platforms Inc., containing historical stock prices.
   - **Sentiment Data:** Extracted from news articles, categorized, and quantified into sentiment scores.

2. **Data Preparation:**
   - Cleaning and normalizing data.
   - Engineering features such as sentiment scores for different ESG categories.

3. **Model Training and Evaluation:**
   - Implemented various time series models to forecast stock prices.
   - Evaluated models using metrics like AIC, BIC, and HQIC for model selection.

## Results
- **VARMAX Model:**
  - Best performance with an AIC of 1338.442.
  - Captures complex interdependencies and external influences on stock prices.

- **OLS Model:**
  - Achieved an R-squared of 0.698, indicating a strong relationship between predictors and stock prices.

## Visualizations
- **Time Series Plot:** Shows the relationship between sentiment scores and stock closing prices.
- **Correlation Heatmap:** Illustrates correlations between different features and stock prices.
- **Distribution Plots:** Display the frequency distribution of sentiment scores across different ESG categories.

## Tools and Technologies
- **Programming Languages:** Python
- **Libraries:** TensorFlow, Keras, scikit-learn, statsmodels, Matplotlib, Seaborn, Pandas, Numpy
- **Platform:** Google Colab
- **API:** Alpha Vantage

## Installation and Setup
1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/stock-prediction-esg-sentiment.git
   cd stock-prediction-esg-sentiment
   ```

2. **Install required libraries:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Set up Alpha Vantage API:**
   - Sign up on [Alpha Vantage](https://www.alphavantage.co/support/#api-key) to get your API key.
   - Replace `'Your_key'` in the code with your actual API key.

## Running the Project
1. **Data Collection:**
   - Execute the notebook `EcoStock-ESG-Driven-Market-Predictions.ipynb` to collect and preprocess the stock and sentiment data.
   
2. **Model Training and Prediction:**
   - Run through the notebook to train the different models and generate forecasts.

## Future Work
- Integrate real-time ESG sentiment updates.
- Expand the analysis to multiple companies.
- Incorporate additional data sources such as financial reports and earnings data.

## References
- [Alpha Vantage API](https://www.alphavantage.co/)
- Relevant research papers and articles on ESG and financial modeling.

## Contributors
- Siddharth Singh
- sms10221@nyu.edu

## License
This project is licensed under the GNU General Public License. See the [LICENSE](LICENSE) file for details.
