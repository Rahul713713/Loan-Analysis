# Data Science Techinspire's Loan Analysis : Project Overview
- Created multiple charts,graphs,boxplots,etc. in order to understand how to minimise the risk of losing money while lending to customers.
- Worked on a dataset consisting of 39717 rows of data for 111 different features.
- Performed univariate analysis as well as multivariate analysis on various features to understand the importance of every feature.
- Used EDA to understand how consumer attributes and loan attributes influence the tendency of default rate.Thus,helped the company in understanding the driving factors (or
driver variables) behind loan default, i.e. the variables which are strong indicators of default.

# Code and Resources Used
- Python Version: 3.6.0
- Packages: pandas, numpy, matplotlib, seaborn

# Data Cleaning
## After reading the data, I needed to clean it up so that it was usable for our data analysis. I made the following changes and created the following variables:
- Checked whether we have missing data for various cloumns.
- Since,many columns had 33%,65% and even 100% missing values,I deleted those columns as they played no part in deciding the defaulting customers. 
- Extracted the numeric part from the variable employment length.Also,deleted the missing values from the same column. 
- Now, there are broadly three types of variablesin our dataset - 1. those which are related to the applicant (demographic variables such as age, occupation, employment details etc.), 2. loan characteristics (amount of loan, interest rate, purpose of loan etc.) and 3. Customer behaviour variables (those which are generated after the loan is approved such as delinquent 2 years, revolving balance, next payment date etc.).I decided to drop the customer behaviour variables as they are not available at the time of loan application, and thus they cannot be used as predictors for credit approval.
- Also, we will not be able to use the variables zip code, address, state etc. The variable 'title' is derived from the variable 'purpose'.Thus,I got rid of all these variables as well
- Converted loan_status to integer type in order to get the total number of customers who defaulted and who didn't.
- Finally,the remaining columns used for EDA are

 1   id                         
 2   member_id                  
 3   loan_amnt                 
 4   funded_amnt                   
 5   funded_amnt_inv             
 6   term                        
 7   int_rate                    
 8   installment                 
 9   grade                        
 10  sub_grade                   
 11  emp_title                    
 12  emp_length                  
 13  home_ownership               
 14  annual_inc                  
 15  verification_status          
 16  issue_d                      
 17  loan_status               
 18  pymnt_plan                                            
 19  purpose                     
 20  dti                        
 21  initial_list_status          
 22  collections_12_mths_ex_med  
 23  policy_code                   
 24  acc_now_delinq              
 25  chargeoff_within_12_mths    
 26  delinq_amnt                  
 27  pub_rec_bankruptcies        
 28  tax_liens 

# EDA
![loan_status vs term](https://github.com/Rahul713713/Loan-Analysis/blob/master/term.png "loan_status vs term")
![loan_status vs term](https://github.com/Rahul713713/Loan-Analysis/blob/master/purpose.png "loan_status vs purpose")
![loan_status vs term](https://github.com/Rahul713713/Loan-Analysis/blob/master/verification_status.png "loan_status vs verification_status")
![loan_status vs term](https://github.com/Rahul713713/Loan-Analysis/blob/master/int_rate.png "loan_status vs int_rate")

