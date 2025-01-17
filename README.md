# Stock-trends-prediction-with-sentiment-analysis
Our project discusses the correlation between trading sentiment and stock market trends by quantifying the data with data visualization.
Since the news often impacts the stock price fluctuations, we are curious about to what extent the sentiment impacts trading. The project
aims to find whether the news sentiment would make an impact on the daily movement of the S&P 500 index. We collect data from the New York
Times for the news sentiment and the S&P 500 Index from Yahoo Finance as the stock market performance within 1005 days. 

The presentation presumes that news can be used to classify different sentiments 80% of the time. However, many biases and noises may
impact the true result of the research. Various events and the reversed trading nature may cause the exhibition of several opposite results
from our expectations. For instance, the stock market index boomed quickly after the pandemic finished instead of deteriorating as the 
pandemic became more serious. One bias is the event and the other noise is the reversed trading nature that investors tend to bet on the 
reverse of the trend to gain profits. We then adopt the data visualization with the most frequently used words to interpret the news 
sentiment and compare it with the stock market trends, such as TF (term frequency) and IDF (inverse document frequency). 

Specifically, the project deploys Vader & AFINN sentiment to obtain an aggregated sentiment score for each day and employs a linear
regression model to associate with the stock prices. Then we use the bootstrap sampling method to generate the confidence interval for the 
sentiment coefficient. In the model fitting part, we add ridge regression when there is a high degree of multicollinearity. Then we use 
cross-validation to measure the model performance. As a result, we achieved a 95% confidence interval of [-0.162, -0.017] that news 
sentiment does impact the stock market price changes. 

The project also has some inevitable confounders that may influence the results. For instance, insider trading, black swan events, and 
reverse psychology change the stock price without being considered in the model. Additionally, the study lacks context awareness and has a 
limited vocabulary coverage with no negotiation handling. 

