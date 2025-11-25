Objective

The goal of this dashboard is to provide a clear, interactive, and daily-updated view of stock performance using Open, High, Low, Close, Adjusted Close, and Volume data.
It helps users quickly understand price trends, moving averages, daily changes, and trading activity for        Ejected tickers.
 Dataset sed
The dashboard is built using the following fields:
Ticker       Close     Open
Adj Close
Volume
Date
High   Low

Key Measures Created

Several DAX measures were calculated to enable insights:
✔ Latest Close Price
Shows the most recent closing price for the selected ticker/date.
✔ Daily Change
Daily Change = [Latest Close] – [Previous Close]
✔ Daily % Change
Daily % Change = DIVIDE([Daily Change], [Previous Close])
✔ Moving Averages (MA20, MA50)
MA20 = AVERAGEX(LASTN(20, VALUES(Data[Date])), [Close])
MA50 = AVERAGEX(LASTN(50, VALUES(Data[Date])), [Close])
Used to compare short–term and long–term trends.
✔ Cumulative Volume / Returns
Cumulative values to observe long-term progress.

Visuals Included in the Dashboard
🔵 Line Chart – Price Trend with Moving Averages
Shows:
Daily close price
MA20 (short-term trend)
MA50 (long-term trend)
Purpose: Identify trend direction and reversals.
🔴  Column Chart – Daily Trading Volume
Shows daily traded volume in billions. Helps track activity spikes and liquidity.
🟣  KPI Cards
Includes:
Latest Volume
Daily % Change
Closing Price
These KPIs give a quick high-level summary.
🟢 Matrix/Table
Displays:
Last close price
Sum of close
Daily change
Daily % change
Sum of volume
This gives detailed numeric insight for multiple tickers.
🟡  Slicers
To filter dashboard dynamically:
Ticker
Date
Allows interactive comparison of stocks and time periods.Dashboard Workflow (Steps Followed)
1. Imported stock dataset into Power BI.
2. Cleaned data: ensured date format, sorted by date, removed blanks.
3. Created DAX measures:
Daily change
% change
Latest close
MA20 / MA50
Cumulative metrics
4. Built KPIs for summary.
5. Designed line charts for trend analysis.
6. Designed volume chart for trading activity.
7. Designed matrix table to show detailed data.
8. Added slicers for ticker and date selection.
9. Applied consistent theme, alignment, spacing, and labeling.
10. Exported dashboard to PDF for client delivery.

Conclusion
The dashboard provides a clear and insightful view of stock performance, enabling the user/client to:
Track real-time price movement
Compare daily and historical trends
Identify bullish/bearish signals with moving averages
Understand trading activity with volume analysis
Quickly filter and analyze multiple tickers

This dashboard is suitable for daily monitoring, reporting, and investment decision support.





