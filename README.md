## Introduction

A couple years ago when I started investing in stock market, my main objective was to learn how online trading of stock works because many of my friends and family 
were talking about it. Once I started having multiple transactions, I decided to keep the trading info in a spreadsheet and Google Sheet was chosen because it is not only free, but also
accessable anytime anywhere. I then also learned about **GOOGLEFINANCE** and used it to automate the retrival of stock info.  However, for some reasons, after using it for a while for 
stocks in Hong Kong and Shanghai-Hong Kong Stock Connect, GOOGLEFINANCE stopped working for those stocks in Shanghai-Hong Kong Stock Connect.  Furthermore, when the spreadsheet gets larger, the refresh might take a long time and 
GOOGLEFINANCE might not work when retriving stock quotes due to various reasons. 

Because of all these reasons, I have to look for an alternative. After checking various solutions on the Internet without very satisfactory results, I decided to 
create a solution myself. I find that **IMPORTXML** is a viable solution for this situation and apparently quotes from **The Wall Street Journal** is quite comprehensive and up to date.

---

## Stock Portfolio Tracker

Stock Portfolio Tracker is a Google Sheet that tracks stock performance.  It uses the **IMPORTXML** buildin function to fetch stock information from https://quotes.wsj.com/. The tracker 
has the following features:

1. It has a **Summary** sheet to provide summary information of all the stocks
2. Each **Stock** portfolio will be placed in a separate stock sheet.  To create a stock sheet, user needs to provide the **path** to the stock's URL from the https://quotes.wsj.com/ 
   to create the stock sheet
3. A custom menu **Stock Quotes** that stores custom functions which currently includes
  * Force Reload Data (fetch stock info in the current stock sheet)
  * Force Reload All Data (fetch stock info of all the stock sheet in the Google Sheet)
  * Create New Stock Sheet (create a new stock sheet with the path to the stock's URL in WSJ)

---

## Usage

Add a new stock sheet:

1. From the **Stock Quotes** menu and choose **Create New Stock Sheet**.  It will ask for the **path** of the stock from the https://quotes.wsj.com/ site.  
   E.g. for Apple Stock at https://quotes.wsj.com/US/XNAS/AAPL, the **path** is **US/XNAS/AAPL**.
2. A sheet based on a template and named after the Stock Symbol will be created.  It will also fetch the latest stock price and relevant information of the stock.

---

## Clone a repository

