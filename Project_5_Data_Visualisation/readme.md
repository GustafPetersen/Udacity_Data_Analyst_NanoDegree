# (Dataset Exploration Title)
## by (your name here)


## Dataset

The goal of this presentation is to showcase my findings from my investigation of Prosper Loan Data.
From the data, I wanted to investigate which factors influenced borrower rate, as it is central for both lenders in Prospers peer-to-peer service, the company Prosper, and the borrowers. The borrower rate has to reach an equilibrium where the rate is profitable for Prosper and Lenders while the cost is not to expensive for borrowers.
Thus the investigation is to determine what factors affect the borrower rate and its variation.


The dataset had 80 columns and 113'937 rows.
The investigation first started with filtering out variables based on the variable definitions sheet.
The initial list of variables set out to explore where:

Credit Grade, Term, Borrower Rate, Estimated Loss, Estimated Return, Prosper Rating (numeric), Prosper Rating (Alpha), Prosper Score, Listing Category, Stated Monthly Income, Occupation, Listing Category, Occupation, EmploymentStatus, Employment Status Duration, Credit Score Range Lower, Credit Score Rang upper, Debt to Income Ratio, Income Range, Stated Monthly Income

But after some investigation into the quality of the data for the aforementioned variables, I ended up only keeping:
ListingCategory, Occupation, BorrowerRate, EstimatedLoss, EstimatedReturn, ProsperRating (Alpha), StatedMonthlyIncome, and DebtToIncomeRatio.

There was a little data wrangling such as changing listing category, which needed to first be changed from numerical values into the categories that we're accompanied and explained in the definitions sheet mentioned earlier.
Prosper Rating was ordered according to lowest to highest ranking: HR, E, D, C, B, A, AA.

Listing Category and Occupation were both concatenated to only include the top 5 most occurring categorical values.


## Summary of Findings

The biggest take away is that Estimated Loss may hugely affect which Prosper Rating a borrower receives, which obviously then affects the Borrower Rate. Initially, I thought that the Estimated Return would have had the strongest correlation, which it proved not to be the case. Most surprisingly however, was the low correlation of Stated Monthly Income in regards to Borrower Rate. I had assumed that the income would affect the rate more.


## Key Insights for Presentation

I chose the plot that seemed the most relevant for my presentation.
First, a boxplot and violinplot above and under each other, displaying the relationship between prosper rating and borrower rate.
Second, a two-dimensional histogram or heatmap, showing the relationship between estimated loss and borrower rate.
Third, another heatmap, showcasing the relation between estimated return and borrower rate.
Fourth, faceted plots displaying again the relationship between estimated loss and borrower rate, however, with the dimension of the relation per Prosper rating, which was interesting.
Finally, a correlational heatmap indicating the Pearson coefficient between the quantitative variables used in the analysis.
