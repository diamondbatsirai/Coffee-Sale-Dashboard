# Coffee-Sale-Dashboard

# Description

This project provides an interactive dashboard to gain actionable insights from coffee sales data. Explore trends in sales volume, revenue, and customer demography’s.

Firstly, I gathered customer data using the XLOOKUP function.
## For Customer Name:

=XLOOKUP(C2,customers!$A$1:$A$1001,customers!$B$1:$B$1001,,0)

## For Customer Email:

=IF(XLOOKUP(C2,customers!$A$1:$A$1001,customers!$C$1:$C$1001,,0)=0,"",XLOOKUP(C2,customers!$A$1:$A$1001,customers!$C$1:$C$1001,,0))

