## Stock Portfolio Tracker

Stock Portfolio Tracker is a Google Sheet that tracks stock performance.  It uses the IMPORTXML buildin function to fetch stock information from https://quotes.wsj.com/. The tracker 
has the following features:

1. It has a **Summary** sheet to provide summary information of all the stocks
2. Each **Stock** portfolio will be placed in a separate stock sheet.  To create a stock sheet, user needs to provide the stock's URL from the https://quotes.wsj.com/ to create the stock sheet
3. A custom menu **Stock Quotes** that stores custom functions

---

## Usage

Add a new stock sheet:

1. From the **Stock Quotes** menu and choose **Create New Stock Sheet**.  It will ask for the **path** of the stock from the https://quotes.wsj.com/ site.  
   E.g. for Apple Stock at https://quotes.wsj.com/US/XNAS/AAPL, the **path** is **US/XNAS/AAPL**.
2. A sheet based on a template and named after the Stock Symbol will be created.  It will also fetch the latest stock price and relevant information of the stock.

---

## Clone a repository

