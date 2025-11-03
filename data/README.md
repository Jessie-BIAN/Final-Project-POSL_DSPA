Dataset 1:  HSall_members.csv

Dataset: Voteview – Members of Congress Data
File used: HSall_members.csv
Provider: Keith T. Poole, Howard Rosenthal, and Voteview.com
This dataset is downloaded from the official Voteview data repository, which provides comprehensive information on members of the U.S. Congress since the First Congress (1789). It contains member-level attributes and ideological scores derived from roll-call voting records.

Conceptual Background
DW-NOMINATE (Dynamic Weighted NOMINAl Three-Step Estimation) is a spatial scaling method developed by Keith Poole and Howard Rosenthal. It positions legislators in a multidimensional ideological space based on their roll-call voting behavior.
The first dimension (Dim1) typically represents the economic liberal–conservative continuum.
The second dimension (Dim2) captures social or regional differences, such as North–South divisions in earlier Congresses.

Relevance to Research Question
This dataset is used to analyze whether the 2010 Supreme Court ruling Citizens United v. FEC — which expanded corporate political spending through Super PACs — led to measurable shifts in the ideological positions of U.S. legislators.
Specifically, we examine changes in DW-NOMINATE Dim1 (economic redistribution ideology) before and after the ruling (comparing pre-2010 and post-2010 Congresses).


Dataset 2: Federal Election Commission – Super PAC Expenditures (all_superpac.rds)

Dataset: Federal Election Commission – Super PAC Expenditures
File used: all_superpac.rds
Provider: Federal Election Commission (FEC)

This dataset was compiled from the official Federal Election Commission (FEC) campaign-finance disclosure archives, which provide Super PAC data only as separate annual or election-cycle files. Each file contains financial and organizational information on political committees registered for that specific year.

Conceptual Background
Super Political Action Committees (Super PACs) are independent-expenditure-only committees that can raise and spend unlimited amounts of money to influence elections, provided their spending is not coordinated with candidates or parties. Their rise followed the Citizens United v. FEC (2010) Supreme Court decision, which expanded corporate and individual rights to make independent political expenditures. Super PACs have since become a central component of U.S. campaign finance, reflecting the growing role of money in electoral politics.

Source and Construction
Because the FEC database releases Super PAC records separately for each year or election cycle, we manually collected, cleaned, and merged all available annual datasets from 2000 to 2024 to create a consistent panel suitable for longitudinal analysis. The final consolidated dataset was saved as all_superpac.rds.

Each year’s file was downloaded from the official FEC data portal (https://www.fec.gov/data/browse-data/?tab=bulk-data
) and standardized into a unified structure before being appended into a single dataset. The dataset includes variables such as committee name and ID, party affiliation, total receipts, total disbursements, independent expenditures, number of donors, average donation, and election cycle.

Relevance to Research Question
This dataset is used to measure the evolution of independent political spending in the United States and to assess how financial flows through Super PACs changed before and after the Citizens United decision. By tracking Super PAC fundraising and expenditure patterns from 2000 to 2024, the dataset provides empirical evidence on the extent to which expanded corporate and individual spending has contributed to partisan and ideological polarization in U.S. politics.
