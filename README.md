# Effects of ProsperLoan Characterics on Various Features
## by Emmanuelaudu Joshua


## Dataset

> The final dataset after preparation contains 83,982 loans with 16 features (including LoanOriginalAmount, LoanStatus, BorrowerState, BorrowerAPR, StatedMonthlyIncome, ProsperRating (Alpha), Occupation, EmploymentStatus, year, month, day, time). The original dataset can be found <a href="https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv">here</a>.


## Summary of Findings

> I'm most interested in figuring out what features are best determining how the total loan amount either negatively or positively affects the BorrowerAPR of the loan. I also would examine other features that would affect the BorrowerAPR,  EmploymentStatus, ProsperRating, StatedMonthlyIncome, LoanStatus and LoanOriginalAmount.
>* The distribution of the LoanStatus showed that about 89% of all Prosper loans are either current or completed which we can assume that they have good profiles. Also, about 8% of Prosper's loans were charged-off or defaulted. Moreover, the remaining 2.4% of loans has the status Past Due and was grouped under a single status: Past Due.
>* The distribution of the LoanOriginalAmount showed significant spikes can be seen at certain price levels(10k,15k,20k,25k), in this visualization, with the most significant spike being at 15k. Which means more of these loan amounts were taken compared to others.
>* The distribution of the StatedMonthIncome is skewed to the right with the StatedMonthlyIncome less than $25k and peaked above 7k borrowers, which shows the majority of borrowers earns below $25K monthly.
>* The distribution of the ProsperRating(Alpha) shows majority of borrowers inbetween D to A. `ProsperRating` grades borrowers on a scale of `AA`(the lowest risk) to `HR`(the highest risk).  Which means not many borrowers and High risk nor are completely at the lowest risk level.
>* The distribution of APR looks multimodal. A small peak centered at 0.1, a large peak centered at 0.2. There is also a small peak centered 0.3. Additionally, there is a very shape peak between 0.30 and 0.40. Only very few loans have APR greater than 0.40. 
Also, the correlation coefficient of BorrowerAPR and LoanOriginalAmount are negatively correlated which further confirms the hypothesis that the more the loan amount, the lower the BorrowerAPR. The LoanOriginalAmount is positively correlated with the StatedMonthlyIncome, it makes sense since borrowers with more monthly income could loan more money.
>* The LoanOriginalAmount increases with higher ProsperRating. The BorrowerAPR decreases with higher ProsperRating. The relationship between BorroweAPR and LoanOriginalAmount turns from negative to slightly positive when the ProsperRating increases from HR to A or better. This may because people with A or AA ratings tend to borrow more money, increasting APR could prevent them borrow even more and maximize the profit. But people with lower ratings tend to borrow less money, decreasing APR could encourage them to borrow more.


## Key Insights for Presentation

> For the presentation, I just focus on features that could affect the borrower APR, which are original loan amount, Prosper rating, Employment Status, LoanStatus. I started by showing the distribution of the loan status. Then, I showed the distribution of the Borrower APR. I showed the relationship of the Year vs LoanOriginalAmount.  I also investigated what months do certain people take loans the most based on EmploymentStatus and finally how the ProsperRating have  effects on relationship of BorrowerAPR and LoanOriginalAmount.