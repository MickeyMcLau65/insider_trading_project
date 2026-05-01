# SEC Insider Trading Analysis Using Malloy

## Project Overview

I was curious whether corporate insiders appear to trade in a way that reveals meaningful patterns about confidence, timing, and ownership behavior. To investigate this, I analyzed SEC Form 3, 4, and 5 ownership filing data using Malloy. These filings report insider ownership and transactions from company officers, directors, and large shareholders.

The project uses multiple related SEC Form 345 files, including submission records, reporting owner information, non-derivative transactions, derivative transactions, holdings, signatures, and footnotes. By combining these tables, I was able to move beyond simple transaction counts and explore who is trading, what companies are involved, what types of transactions dominate, and how insider activity changes over time.

## Data and Tools

The dataset includes SEC ownership filing data from EDGAR. I used Malloy to define sources, join related tables, and query the data. I also used Visual Studio Code to write the Malloy files and GitHub to host the final project.

Key files used include:

- `SUBMISSION.tsv`
- `REPORTINGOWNER.tsv`
- `OWNER_SIGNATURE.tsv`
- `NONDERIV_TRANS.tsv`
- `DERIV_TRANS.tsv`
- `NONDERIV_HOLDING.tsv`
- `DERIV_HOLDING.tsv`
- `FOOTNOTES.tsv`

## Questions I Explored

The main question I wanted to answer was: **Do insider transactions reveal meaningful patterns about corporate behavior and investor confidence?**

To answer this, I explored:

1. What types of insider filings are most common?
2. Which companies appear most frequently in the data?
3. Are insiders more often acquiring or disposing of shares?
4. Which companies have the highest estimated insider transaction value?
5. How does insider transaction activity change over time?
6. Are most transactions tied to direct or indirect ownership?

## Key Findings

### Filing activity is concentrated in certain form types

The first thing I looked at was which SEC ownership forms appeared most often. This helped me understand whether the dataset was mostly made up of initial ownership filings, changes in ownership, or annual ownership statements.


The results showed that transaction-based filings were especially important because they reveal changes in insider ownership rather than just static ownership information.

### Insider activity is not evenly distributed across companies

Next, I looked at which companies had the most insider filings.


This showed that insider filing activity is concentrated among certain companies. That matters because high filing counts may reflect larger leadership teams, more equity compensation, or more frequent insider transactions.

### Disposals are more common than acquisitions

One of the biggest findings was that insiders often dispose of shares more frequently than they acquire them.


At first, I expected insider buying to be a major part of the dataset because insider purchases can signal confidence. However, the data showed that selling or disposing of shares is more common. This makes sense because insiders often receive stock-based compensation and may sell shares for diversification, taxes, or liquidity.

### A small number of transactions drive a large amount of value

When I analyzed the largest individual transactions and companies with the highest estimated transaction value, I found that transaction value is highly concentrated.


This was one of the most interesting findings because it shows that counting transactions alone can be misleading. A company may have fewer filings but still represent a much larger dollar value of insider activity.

### Insider transaction activity changes over time

I also looked at insider transaction activity by year.


This helped show whether insider activity was stable or clustered in certain years. Changes over time may be connected to market conditions, company events, executive compensation cycles, or broader economic trends.

## What Surprised Me

The most surprising thing I learned was that insider selling is not automatically a negative signal. Before analyzing the data, I assumed insider selling might suggest a lack of confidence in the company. However, the results showed that selling is very common and may happen for many routine reasons. Insider buying may be more meaningful because it is less common and usually requires the insider to commit personal capital.

## Conclusion

This project showed me that insider trading data is useful, but it needs context. The most valuable insight is not simply whether insiders are buying or selling, but how large the transactions are, which companies are involved, who is reporting them, and whether activity changes over time.

Using Malloy made it easier to connect multiple SEC data tables and build a more complete analysis. Instead of only looking at one transaction file, I was able to combine filing-level information, owner information, signatures, holdings, and footnotes into a broader picture of insider behavior.

## Why are these findings important?

These findings would matter to investors, financial analysts, portfolio managers, and compliance teams. Investors and analysts could use insider buying as one input when evaluating company confidence, while portfolio managers could track insider activity as part of a broader investment research process. Compliance teams could also use this type of analysis to monitor unusual filing patterns, transaction concentration, or ownership changes.

## Project Reflection 

Through this project I was able to learn alot about insider trading, which is something that I have never really looked too into before. I was able to learn some cool things about insider trading and was able to draw analysis on this. Reflecting on this project I thought it was really cool to write the malloy with the help of AI to streamline a process that normally would take a lot more time if AI was not a helpful tool. While this helps it also comes with lots of trouble shooting which was the hardest part of the project, getting AI to complete the troubleshooting efficiently. 