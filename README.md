# Coffee-Sale-Dashboard

# Description

This project provides an interactive dashboard to gain actionable insights from coffee sales data. Explore trends in sales volume, revenue, and customer demography’s.

Firstly, I gathered customer data using the XLOOKUP function.
## For Customer Name:

=XLOOKUP(C2,customers!$A$1:$A$1001,customers!$B$1:$B$1001,,0)

## For Customer Email:

=IF(XLOOKUP(C2,customers!$A$1:$A$1001,customers!$C$1:$C$1001,,0)=0,"",XLOOKUP(C2,customers!$A$1:$A$1001,customers!$C$1:$C$1001,,0))

## For Country:

=XLOOKUP(C2,customers!$A$1:$A$1001,customers!$G$1:$G$1001,,0)

## Product Information.

I gathered product information using INDEX function(I populated all the cells at once that is Coffee type, Roast Type, Size and Unit Price.

=INDEX(products!$A$1:$G$49,MATCH(orders!$D2,products!$A$1:$A$49,0),MATCH(orders!I$1,products!$A$1:$G$1,0))

## Sales Column

I calculated Sales column by the formula =L2*E2 and drag down to fill the whole column

# Insertion of new Columns

I inserted Coffee Type Name so that the audience understand rather than the abbreviations.
I inserted Roast Type Name to show the full names of the abbreviations for better understanding.
I inserted Loyalty cards, which is needed to find out how many customers have it.



