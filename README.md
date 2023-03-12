# (Dataset Exploration Title)
## by (your name here)


## Dataset

> Provide basic information about your dataset in this section. If you selected your own dataset, make sure you note the source of your data and summarize any data wrangling steps that you performed before you started your exploration.

The dataset comprises data on 113937 loans with 81 attributes corresponding to the loan, borrower and lender's details. 61 columns are numeric including the key/id columns and categorical types for ListingCategory. The columns include, amoung others; BorrowerRate, EmploymentStatus, IncomeRange, LoanOriginalAmount. The dataset covers juist over 9 years between 2005 and 2014.

There were huge outliers for the StatedMonthlyIncome attribute that skewed the data, all values greater than $20,000 were removed from the dataset.


## Summary of Findings

From the univeriate analysis, The distribution of LoanStatus revealed "Current" had the highest count of Loans, further investigations revealed LoanListing were in an increasing sequence with the highest count having been made in 2013, the last full year in the dataset. A bivariate plot of LoanStatus against LoanComencementYear revealed the majority of the LoanListing were made in the last 3 years of the dataset. 77% of the LoanListing were of Term length 36months, and a bivariate plot against LoanStatus revealed the majority of the loans were "Current" or overaly still active, with the exception of the 12 month Term which had a zero count on active Laons.

The highest count of Loans for IncomeRange was at "25k-50k", with over 25% of the individuals earning over $25,000. This was matched with the StatedMontlyIncomes with a right tailed distribution with a peak at $3,500 and 75% of the incomes lie below \\$6,825. Ploting Income levels againt LoanStatus reaveled the highest count for each income level were Current on their monthly payments or in the FinalPaymentsInProgress level.


The majority of the loans are of below $10,000 in value and the appear to peak, in somewhat of a decreaasing sequence.
Loans listed for individuals with higher incomes appear to be moslty in a positive outcome, especially those of above \\$25,000 offered for Income level above $7,500. While generally large loans(>$15,000) tend to have a positive outcome, loans that were either Cancelled, Defauled or Charged of were from lower Income levels, (<\\$2500). There is a floor Income amount for loans above \\$25,000.

Amoung those that provided their occupation, the top five occupations are Professional, Sales, Computer Programmer, Executive and Teacher.
The most popular list category is category 1:Debt Consolidation.
On average across EmploymentStatus, more loans were issued to Employed and Fulltime individuals on each level.
1-DebtConsolidation has the highest counts for ListingCategory. Ploting ListingCategory against LaonSTatus reveales the highest counts are mostlty distributed between "Past Due (61-90days)" (40,000) and "Past Due (15-30days)" (11,000).

The distribution for BorrowerAPR is unimodal, with an upward trend with multiple peaks. The higher the mean BorrowerAPR, the higher the chances the loan is in an unfavourable LoanStatus(i.e Past Due, Defaulted and ChargedOff). Loan Original Amount is negatively correlated with BorrowerAPR, the higher the loan, the lower the percentage cost.

In the heatmap of 3 varibales; 'LoanStatus', 'Term' and'BorrowerAPR', here is a conistant pattern accross loan Term for all level of LoanStatus category, where lower BorrowerAPR are in the 3 levels; Current, Completed and FinalPaymentInProgress. Higher BorrowerAPR for all Term lenth are typically in the 3 levels Defaulted, ChargedOff or Past Due.

Ploting MonthlyPayments against Term, the violin plots show the median payment is generally the same with the distribution for 12 month Term having a long tail.


Plotting 'LoanComencementYear', 'StatedMonthlyIncome', and 'LoanStatus' on a clustered barchart, we discover on average accross the years, Higher incomes correspond to Completed and current Loans, whereas Lower incomes  corresponds to Past Due and Defauled loans.

On the heatmap for 'LoanStatus', 'ListingCategory' and 'LoanOriginalAmount' we see the amount for Business Loans(Listing category 3) was generally high accross all levels of LoanStatus, which is typical of business loans. And despite the amount, they were about equaly like to fall into any of the outcome categories.Student Loans(5) and Personal loans(4) were of the lowest amounts, and there weren't any active loans from either levels. For every level of LoanStatus There is a Debt consolidation Loan(1), this is consistant with this category being the most common ListingCategory. What is interesting is loans with least amount were the ones that were cancelled. 


## Key Insights for Presentation

The presantation is going to focus on how LoanStatus interacts with Term, BorrowerAPR LoanOriginationYear as well as numeric variable of StatedMonthlyIncome and LoanOriginalAmount. Monthly incomes are going to be limited to those below $20,000, which is about 99% of the dataset. We will begin by investigating the distributions of each indivdual variable and proceed to how they relate to each other.

The highest count of loan are in the "Current" loan status and 77% of all loans were used for a 36 month Term period. There were more loans listed each successive year, with 2013 having the highest count of loans, the majority of these were current on the payments. The distribution for BorrowerAPR is unimodal, and the higher the BorrowerAPR, the higher the chance the loan will result in an unfavourable outcome.  The is a floor income amount for loans above \\$25,000, and the majority of these are 'Current' on their repayments.

