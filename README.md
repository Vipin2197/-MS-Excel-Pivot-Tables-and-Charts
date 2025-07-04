# Kickstart-CrowdFunding MS-Excel-Pivot-Tables-and-Charts
 Excel Data Model & Sheets
Projects: key columns like project_id, name, category, country, launched_at, deadline, goal_usd, pledged_usd, backers, state.

Currency: includes exchange rates to USD.

Calendar: use formulas (from launched_at converted from Unix timestamp) to derive Year, Month, Quarter, YearMonth, Weekday, FinancialMonth, FinancialQuarter 
experienceleague.adobe.com


📈 Core Analyses & Formulas
Unix timestamp conversion: =(launched_at/86400)+DATE(1970,1,1) for readable dates 


Pct Funded: =pledged_usd/goal_usd.

Avg Donation: =IFERROR(pledged_usd / backers,0) 


Split Categories: use text functions to separate primary/sub-category 


Goal Buckets: use COUNTIFS across goal ranges for success/fail counts 


🗂️ Pivot Tables & Charts
Campaign state by category: Pivot table + stacked column chart (filterable by country) 


State by sub-category: filtered cart by country + parent category 


Timeline pivot: count by state over launch date (grouped by Year/Month) + line chart 
medium.com
.

Goal vs Success: sheet with goal bands, counts, % success/fail/cancel; then a line chart 


Summary stats: mean/median/std dev of backers for successful vs failed campaigns 


📊 Dashboard Components
Slicers for country, category, launch date.

Pivot charts: stacked, line, and scatter (goal vs % success).

Conditional formatting: color-scale for % Funded, state-based coloring.

📌 High-Impact Business Insights
Best launch months: May–July show ~60%+ success 


Category success: Music shows ~77% success; subcategories like “Plays” exhibit high volatility 

Goal recommendation: Projects under $5K have notably higher success rates 
gcsu.edu


Backer metrics: Early pledge momentum and average donation help differentiate success vs failure.

Data limitations: small sample (~4K), heavy US bias, potential domain-specific skew

 Screenshots / Demos

view : ![dashboard preview]![Screenshot 2025-07-02 113238](https://github.com/user-attachments/assets/313a3e53-1cb0-459a-aebc-ac0c98a047f7)
