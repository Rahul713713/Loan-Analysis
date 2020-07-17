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
 0   id                         
 1   member_id                  
 2   loan_amnt                 
 3   funded_amnt                   
 4   funded_amnt_inv             
 5   term                        
 6   int_rate                    
 7   installment                 
 8   grade                        
 9   sub_grade                   
 10  emp_title                    
 11  emp_length                  
 12  home_ownership               
 13  annual_inc                  
 14  verification_status          
 15  issue_d                      
 16  loan_status               
 17  pymnt_plan                  
 18  url                          
 19  purpose                     
 23  dti                        
 24  initial_list_status          
 25  collections_12_mths_ex_med  
 26  policy_code                   
 27  acc_now_delinq              
 28  chargeoff_within_12_mths    
 29  delinq_amnt                  
 30  pub_rec_bankruptcies        
 31  tax_liens 
