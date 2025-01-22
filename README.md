# Lending Club Case Study:
>   This project focuses on analyzing data from a consumer finance company that provides loans to urban customers. The goal is to       identify patterns in the profiles of past loan applicants to predict the likelihood of default. By understanding these patterns, the company can make informed decisions, such as denying loans, reducing loan amounts, or offering loans to risky applicants at higher interest rates. This helps balance the risks of financial loss due to defaults and the loss of business opportunities from overly         conservative approvals.


## Table of Contents:
* [objective](#objective)
* [Dataset](#Dataset)
* [Technologies Used](#Technologies-Used)
* [Key Insights](#Key-Insights)
  
## Objective:
    The objective of this case study is to identify risky loan applicants to help reduce credit loss. By understanding the driving factors behind loan defaults and identifying strong indicators of default, the company can improve its portfolio management and risk assessment strategies.

## Dataset: loan.csv
    Some of the variables used for this project are as follows:
        1. issue_d - The month which the loan was funded
        2. emp_length - Employment length in years. Possible values are between 0 and 10 where 0 means less than one year and 10 means ten or more years. 
        3. int_rate - Interest Rate on the loan
        4. revol_util - Revolving line utilization rate, or the amount of credit the borrower is using relative to all available revolving credit.
        5. default (derived column) - Derived from categories of loan_status such as Charged off, Fully Paid and Current.
        6. loan_amnt - The listed amount of the loan applied for by the borrower. If at some point in time, the credit department reduces the loan amount, then it will be reflected in this value.
        7. loan_status - The listed amount of the loan applied for by the borrower. If at some point in time, the credit department reduces the loan amount, then it will be reflected in this value.
        8. grade - LC assigned loan grade
        9. purpose - A category provided by the borrower for the loan request. 
        10.term - The number of payments on the loan. Values are in months and can be either 36 or 60.
        11.home_ownership - The home ownership status provided by the borrower during registration. Our values are: RENT, OWN, MORTGAGE, OTHER.
        12.verification_status - Indicates if income was verified by LC, not verified, or if the income source was verified
        13.dti - A ratio calculated using the borrower’s total monthly debt payments on the total debt obligations, excluding mortgage and the requested LC loan, divided by the borrower’s self-reported monthly income.

## Technologies Used:
- pandas 
- numpy 
- seaborn
- matplotlib
- plotly
- datetime
- warnings 

## Key Insights:
- 14% of the loans are defaulted.
- Average loan Amount is higher for defaulted loans.
- Loans have increased significantly year over year.
- Debt consolidation loans have increased year over year and highest in 2011.
- Highest number of loans are for Debt Consolidation, followed by Credit_card, Other and Home Improvement.
- Based on the data available and analysis, the top 5 driving factors (driver variables) which indicate if a person is likely to default are: 
	1. Purpose 2. Term 3. Grade 4. Interest Rate 5. Employment Length
- Small business has highest percentage of defaults
- Renewable energy has the second highest default rate
- Educational has the third highest default rate
- Highest default rate is for 60 months Term
- Highest default rate is for Grade G
- Default % is increasing with increase in Grade
- Highest default rate is for interest rate range 20%-25%
- Default % is increasing with interest rate
- Highest number of defaulted loans percentage are for Employment Length not available (No Info)
