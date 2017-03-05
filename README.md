# data-science
# get the stock price from Yahoo Finance
# method reference https://www.analyticsvidhya.com/blog/2016/02/time-series-forecasting-codes-python/

import pandas as pd
import pandas_datareader.data as web
import datetime

start = datetime.datetime(2016,3,5)
end = datetime.date.today()

google = web.DataReader("GOOG", "yahoo", start, end)
 
google.head()
