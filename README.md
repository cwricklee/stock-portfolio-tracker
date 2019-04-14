## Introduction

A couple years ago when I started investing in stock market, my main objective was to learn how online trading of stock works as many of my friends and family members 
were talking about it. Once I started having multiple transactions, I decided to keep the trading info in a spreadsheet. Google Sheet was chosen because it is not only free, but also
accessable anytime anywhere. I then learned about **GOOGLEFINANCE** and used it to automate the retrival of stock quotes.  However, for some unknown reasons, after using it for a while for 
stocks in Hong Kong Stock Exchange and Shanghai-Hong Kong Stock Connect, GOOGLEFINANCE stopped working for those stocks in Shanghai-Hong Kong Stock Connect.
Furthermore, when the spreadsheet gets larger, the refresh takes a long time and even fails occasionally when retriving stock quotes.   

Because of all these reasons and after checking various solutions on the Internet without very satisfactory results, I decided to 
create a solution myself. I find that using **IMPORTXML** is a viable and simple solution for this situation and apparently stock quotes from **The Wall Street Journal** is quite comprehensive 
and up to date.

---

## Stock Portfolio Tracker

Stock Portfolio Tracker is a Google Sheet that tracks stock performance.  It uses the **IMPORTXML** buildin function to fetch stock information from https://quotes.wsj.com/. The tracker 
has the following features:

1. It has a **Summary** sheet to provide summary information of all the stocks.
2. Each **Stock** portfolio will be placed in a separate stock sheet.  To create a stock sheet, user needs to provide the **path** to the stock's URL from the https://quotes.wsj.com/ 
   to create the stock sheet.
3. A custom **Stock Quotes** menu which includes functions to 

   * Force Reload Data (fetch stock info in the current stock sheet)
   * Force Reload All Data (fetch stock info of all the stock sheets in the Google Sheet)
   * Create New Stock Sheet (create a new stock sheet with a given path to the stock's URL in WSJ)

---

## Usage

### Get a copy of the spreadsheet:

1. Get a copy of the Google Sheet [here](https://docs.google.com/spreadsheets/d/17G_i9EVb06CQ74aik3Bh0vuXqvS6nm-mufse0-apAMI/edit?usp=sharing) and open in Google Chrome browser.
2. Login to Google account to access the full functionality of the Google sheet.
3. Under the **File** menu, click **Make a copy...** to create a copy to keep track of personal stock transations.

### Add a new stock sheet:

1. From the **Stock Quotes** menu, choose **Create New Stock Sheet**.  It will ask for the **path** of the stock from the https://quotes.wsj.com/ site.  
   E.g. for Apple Stock at https://quotes.wsj.com/US/XNAS/AAPL, the **path** is **US/XNAS/AAPL**.
2. A sheet based on a template and named after the Stock Symbol will be created.  It will also fetch the latest stock price and relevant information of the stock.
3. To add this stock details to the Summary sheet, click the **Add to Summary** button.

---

## Disclaimer

As I am a casual investor with very limited knowledge in trading, the terminology and calculations used are simply based on my own understanding.
This software is provided as is and I make no representations or warranties of any kind concering the safety, suitability, lack of viruses, inaccuracies, typographical errors,
or other harmful components of this software.  I will not be liable for any damages you may suffer in connection with using, modifying, or distributing this software.

## Special Notes

1. This project uses Google Apps Script which is part of Google OAuth web clients.  All Google OAuth web clients require verification by Google and seems a bit complicated in my situation. I therefore didn't go through the whole process.
For this reason, users might see an *unverified app* screen when they try to authorized my script.
2. In the Stock Transaction sheet, rows 15-20 are hidden with some sample transactions. These transactions are for reference only and they are not included in the calculations.
