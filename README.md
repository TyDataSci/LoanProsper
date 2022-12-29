
# Communicate Data Findings 

# LoanProsper
In this <a href='https://github.com/TyDataSci/LoanProsper/blob/master/visualization.ipynb'> notebook</a>, I will explore the Prosper Loan dataset that can be downloaded by clicking here. Prosper was the first peer-to-peer lender in the United States and since 2005, Prosper has facilitated more than $18 billion in loans to more than 1,080,000 people. The Prosper Loan dataset details 113937 loans lent by Prosper from 2005 to 2014.

# Summary of Findings
### Loan Status 
The overarching question of this analysis is what causes a lendee to default on a loan. 
The Loan Status is categorized by Current , Completed , Chargedoff , Defaulted ,Past Due by time period, and Final Payment In Progress. For the purposes of my analysis, I focused on the 3 loan statuses of Defaulted, Chargedoff , and Completed. 
Defaulted and Charged Off loans are loans that have gone that are more than 120 days past due on their payments and outstanding debts deemed uncollectible. By combining Defaulted loans with Chargedoff loans, I was able to make a comparison betweeen Bad Standing Loans and those Completed in full. 

### Loan Original Amount
The loans found in this dataset skews heavily in favor of smaller loans of less than 15,000 USD. For Bad Standing Loans, 91% of loans are under 15,000 USD and 89% of all Completed Loans were under 15,000 USD.
 as the Credit Score increased the reason that loans ended in default had less to do with the Borrower APR and more related to the size of the Loan Amount. For individuals in Bad Standing as their Credit Score increased their loan amount greatly increased.
 In many cases the Borrowing Rate nears zero percent APR for very high loan amounts. This would likely be situations such as Auto Loans or other high priced sales financed at extremely low rates to incentivize a purchase.
### Borrowers Annual Percentage Rate
Borrower APR looks to be a key contributor to the liklihood of a loan never being paid off and finishing in Bad Standing. 70% of all Bad Standing Loans occurred when the Borrower APR was 0.3 to 0.4.
omparatively only 44% of the Completed loans occurred when the Borrower APR was 0.3 to 0.4. Borrower APR looks to be a key contributor to the liklihood of a loan never being paid off and finishing in Bad Standing
### Credit Score of the lendee
Lendees receiving loans they were unable to to return had lower Credit Scores in comparison to the Completed Loans. 65% of Bad Standing Loans had a Credit Score lower than 750, compared to 56% of the Completed Loans.
Creidit Score had a strong relationship with Loan amount, finding that for every 1 point the Credit Score increased the Loan Amount increases by 37.10 USD.
Individuals of higher Credit Score were more likely to receive high loan amounts and this was the strongest reason for individuals of high Credit Scores to end up defaulting on there loans.

### Estimated Return of the loans.
Estimated Return is maximized for individuals whose Credit Scores were on the lower end, near 650, from there it consistently decreases as Credit Score increases.
The Estimated Return held a strong positive wit the Borrower APR increased and it was strongest among the featured variables For every 0.1 percent the Borrower APR increases, the Estimated Return Increases by 0.03 points.
Estimated Return maximizes near 0.35 APR. Due to the increase in Estimated Returns, the lenders were economically incentivized to lend smaller amounts of money and the lendee most willing to accept higher APR's were also individuals of lower Credits Scores.

## References
- https://seaborn.pydata.org/generated/seaborn.lmplot.html
- https://stackoverflow.com/questions/14032521/python-data-structure-sort-list-alphabetically
- https://stackoverflow.com/questions/44098362/using-mpatches-patch-for-a-custom-legend
- https://stackoverflow.com/questions/27019079/move-seaborn-plot-legend-to-a-different-position
- https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.legend.html
- https://matplotlib.org/stable/gallery/color/named_colors.html
- https://stackoverflow.com/questions/54781243/hide-legend-from-seaborn-pairplot
- https://stackoverflow.com/questions/49907455/hide-code-when-exporting-jupyter-notebook-to-html
- https://nbconvert.readthedocs.io/en/latest/usage.html
