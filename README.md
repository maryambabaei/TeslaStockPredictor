
### 📈 Tesla Stock Price Prediction

This project analyzes and predicts Tesla, Inc.'s stock prices using machine learning models. The dataset spans from **January 2012 to December 2020**, containing **over 2,500 daily entries** with features such as:

- Open, High, Low, and Close prices  
- Trading Volume  
- Market Capitalization  
- Outstanding Shares

I applied both **univariate** and **multivariate** time series forecasting techniques:

#### 🔹 Univariate Models
Focused solely on the "Close" price, I used:
- Simple RNN  
- LSTM  
- GRU  

#### 🔹 Multivariate Models
Incorporated additional features, particularly "Open" and "Close" prices, using:
- LSTM  
- GRU  

However, the multivariate models underperformed, showing high **MAE** and **MSE**, along with low **R² scores**. These results suggest the models, especially the multivariate GRU, struggled to capture the underlying stock price dynamics.

#### ⚠️ Observations
Several factors may have affected model performance:
- Lack of data shuffling introduced potential bias  
- Limited training epochs may have prevented convergence  
- Stock price movements are inherently complex and influenced by external factors not captured in the dataset
