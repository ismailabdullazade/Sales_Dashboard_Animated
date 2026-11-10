# Sales Dashboard - Power BI Project (.pbip)

## Open it
1. Use the latest Power BI Desktop (Windows).
2. File > Options and settings > Options > Preview features: enable
   "Power BI Project (.pbip) save option" and "Store semantic model using TMDL format"
   (and "Store reports using enhanced metadata format (PBIR)" if listed). Restart Desktop.
3. Unzip this folder, then double-click `SalesDashboard.pbip`.
4. Click Home > Refresh once. Data is embedded in the model (sample data), no source needed.
5. File > Save as to get a regular .pbix if you want a single file.

## Pages
- Overview: KPI cards, slicers, trend with Revenue/Profit bookmark toggle, region/category/product visuals.
- Trends: year-over-year lines, ribbon chart, product matrix with YoY growth, margin by year.
- Animated Explorer: scatter chart with Play Axis (Month Year). Click the play button at the bottom-left of the chart.

## Using your own data
Open Transform data, replace the `Sales` query with your source, keep columns
OrderDate, Category, Product, Region, Units, Revenue, Cost.

## If something does not load
- If Desktop reports an error about bookmarks, delete `SalesDashboard.Report/definition/bookmarks`
  and recreate the two bookmarks on the Overview page (hide/show the two trend visuals), then assign them to the two buttons.
- If a visual shows an error, select it and re-drag its fields; the model itself is unchanged.
