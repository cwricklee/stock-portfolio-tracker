## Stock Portfolio Tracker

Stock Portfolio Tracker is a Google Sheet that tracks stock performance.  It uses the IMPORTXML buildin function to fetch stock information from https://quotes.wsj.com/. The tracker 
has the following features:

1. It has a **Summary** sheet to provide summary information of all the stocks
2. Each **Stock** portfolio will be placed in a separate stock sheet.  To create a stock sheet, user needs to provide the stock's URL from the https://quotes.wsj.com/ to create the stock sheet
3. A custom menu **Stock Quotes** that stores custom functions

---

## Usage

Add a new stock sheet:

1. Click the **Stock Quotes** menu and choose **Create New Stock Sheet**.  It will ask for the **path** of the stock from the https://quotes.wsj.com/ site.
2. A sheet based on a template and named after the Stock Symbol will be created.  It will also fetch the latest stock price and relevant information of the stock.

---

## Clone a repository

Use these steps to clone from SourceTree, our client for using the repository command-line free. Cloning allows you to work on your files locally. If you don't yet have SourceTree, [download and install first](https://www.sourcetreeapp.com/). If you prefer to clone from the command line, see [Clone a repository](https://confluence.atlassian.com/x/4whODQ).

1. You’ll see the clone button under the **Source** heading. Click that button.
2. Now click **Check out in SourceTree**. You may need to create a SourceTree account or log in.
3. When you see the **Clone New** dialog in SourceTree, update the destination path and name if you’d like to and then click **Clone**.
4. Open the directory you just created to see your repository’s files.

Now that you're more familiar with your Bitbucket repository, go ahead and add a new file locally. You can [push your change back to Bitbucket with SourceTree](https://confluence.atlassian.com/x/iqyBMg), or you can [add, commit,](https://confluence.atlassian.com/x/8QhODQ) and [push from the command line](https://confluence.atlassian.com/x/NQ0zDQ).