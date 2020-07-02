# KPMG-virtual-internship

I have enrolled to a virtual internship at KPMG, through [InsideSherpa](https://www.insidesherpa.com/virtual-internships/theme/m7W4GMqeT3bh9Nb2c/KPMG-Data-Analytics-Virtual-Internship).

This experience was so much to go through, and I have certainly learned new things, such as working with Tableau.

# Module 1

# Module 2

The task was to create a PowerPoint presentation wihch outlines the approach we will be taking to identify which of the __1000 customers__ *Sprocket Central Pty Ltd* should target, based on this dataset. Explain the three phases:  Data Exploration; Model Development and Interpretation.

The below section was inspired by [Blast analitics](https://www.blastanalytics.com/blog/rfm-analysis-boosts-sales) and code was used with slight modification form [Susan Li's](https://towardsdatascience.com/find-your-best-customers-with-customer-segmentation-in-python-61d602f9eee6) blogpost on Medium.

To find the best customers, the well known RFM matrix principle is the go-to. For this, we will create an additional table using the Transaction sheet (df1), and will create 3 additional datapoints:

    Recency (R) - shows the days since last purchase
    Frequency (F) - cummulative score, how many times a customer made purchase
    Monetary (M) - cummulative score, how much money did a customer spent

Using the above datapoints we will calculate the:

    RFM score, which is used to select the appropriate marketing strategy for each customer group
    
Segment | RFM score | Description | Marketing trategy
---|---|---|---
Best Customers | 111 |Bought most recently and most often, and spend the most |No price incentives, new products, and loyalty programs
Loyal Customers |  	X1X |Buy most frequently|Use R and M to further segment
Big Spenders | XX1 |Spend the most|Market your most expensive products
Almost Lost | 311 |Haven’t purchased for some time, but purchased frequently and spend the most|Aggressive price incentives
Lost Customers | 411 |Haven’t purchased for some time, but purchased frequently and spend the most|Aggressive price incentives
Lost Cheap Customers | 444 |Last purchased long ago, purchased few, and spent little|Don’t spend too much trying to re-acquire
