# Udacity Blog Post

This is a submission for the udancity blog post project 

[blog post](https://medium.com/@alsalman.hn/prospects-of-saudi-stock-market-9776a9a6bec)

# Motivation behined choosing the project 

Coming from a financial background. I have always been fascinated by the stock markets in general and the Saudi Stock market in particular

## Librareis used 

- `requests` : This library was necessary to create the http requests for Tadawul website. 
- `math` : This library was used to round numbers up. 
- `numpy` : numpy is very useful library to create ranges that are used in loops.  
-  `pandas` : pandas was essential for craeting data frames to store the data we scraped in nice and convenient format.  
- `datetime` : important library to minuplate the dates and time. 
- `matplotlib.pyplot` : I used this library to plot the timeseries for the analysis. 


## Creating Parse function 

Since Tadawul does not provide API, I had to create my own. Therefore I started by creating a url parser that craetes http addresses to be sent to the Tadawul server. This is what `url_parser` mainly does. 

## Creating a wrapper function 

Since each request only return 10 records, I had to create a wrapper function to handle the paginations. This is  what `get_index_raw()` mainly does. 

## Creating a clean up function

All the returned data comes as strings. Therefore, it is necessary to correct the types first before proceeding. This could have been done without a specific function. However, it was convienent to bundle all the cleaning up steps into one function. 

## Conclusion

Long term investment in the Saudi stock market does not follow the common wisdom about the stock market as the market is highly volatile. The primary reason for this volatility is the strong relationship between the Saudi economy and the Oil market.

However, the government has been taking initiatives to break this connection. There were number of changes introduced including the leadership of the government as in the example of the appointment of Prince Mohammed bin Salman as the Crown Prince which lead to market shocks. Those shocks create opporutinites for investors to profit.


## Anowledgements

- The Saudi Market Index data was obtained from [Tadawul](https://www.tadawul.com.sa/wps/portal/tadawul/home/) website.

- The oil prices data was obtained from [Quandl](https://www.quandl.com/).


