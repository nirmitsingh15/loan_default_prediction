# Loan Default Prediction Model

## Problem Statement
To predict the loan outcome at the time of application, whether it will be a default case or the loan will be paid on time.

## Data Description:
The dataset provided includes the following files:
- Train Data: Contains details of the loan provided by the lending company.
- Accounts Data: Details of loans taken by the borrower before applying for a loan from the lending company.
- Enquiry Data: Contains details of previous loan applications made by the applicant.


## Features Engineered:

 Below are the engineered features:
 
- **loan_amount**: Total loan amount taken by the borrower
- **total_loans**: Total number of loans taken by the borrower.
- **active_loan**: Number of active loans.
- **inactive_loan**: Number of inactive loans.
- **amount_overdue**: Amount of the loan that is/was overdue.
- **avg_overdue_days**: Average number of days overdue for loans.
- **min_overdue_days**: Minimum number of days overdue for loans.
- **max_overdue_days**: Maximum number of days overdue for loans.
- **overdue_count**: Count of overdue loans.
- **total_payments**: Total number of payments made towards loans.
- **avg_loan_duration**: Average duration of loans.
- **number_of_Consumer_credit**: Number of consumer credit loans.
- **number_of_Credit_card**: Number of credit card loans.
- **number_of_Microloan**: Number of microloans.
- **number_of_Mortgage**: Number of mortgage loans.
- **number_of_Car_loan**: Number of car loans.
- **number_of_other_loan**: Number of other loans.(includes all loans besides top 5 loans on distribution basis(credit card,consumer credit,mortgage,micro loan, car loan))
- **consumer_credit**: Indicator for having a consumer credit loan
- **credit_card**: Indicator for having a credit card loan.
- **car_loan**: Indicator for having a car loan.
- **mortgage**: Indicator for having a mortgage loan.
- **microloan**: Indicator for having a microloan.
- **other_loan**: Indicator for having other type of loan.(includes all loans besides top 5 loans on distribution basis(credit card,consumer credit,mortgage,micro loan, car loan))
- **total_enquiry_amount**: Total amount of loan enquiries made.
- **num_enquiries**: Number of loan enquiries made.
- **loan_enquiry_ratio**: Ratio of loan inquiries to total loans.
- **overdue_perct**: Percentage of loans that are overdue.
- **enquiry_Another type of loan**: Indicator for another type of loan enquiry.
- **enquiry_Car loan**: Indicator for a car loan enquiry.
- **enquiry_Cash loan (non-earmarked)**: Indicator for a non-earmarked cash loan enquiry.
- **enquiry_Cash loans**: Indicator for a cash loan enquiry.
- **enquiry_Consumer credit**: Indicator for a consumer credit loan enquiry.
- **enquiry_Credit card**: Indicator for a credit card loan enquiry.
- **enquiry_Interbank credit**: Indicator for an interbank credit enquiry.
- **enquiry_Loan for business development**: Indicator for a business development loan enquiry.
- **enquiry_Loan for purchase of shares (margin lending)**: Indicator for a loan for the purchase of shares enquiry.
- **enquiry_Loan for the purchase of equipment**: Indicator for an equipment purchase loan enquiry.
- **enquiry_Loan for working capital replenishment**: Indicator for a working capital replenishment loan enquiry.
- **enquiry_Microloan**: Indicator for a microloan inquiry.
- **enquiry_Mobile operator loan**: Indicator for a mobile operator loan enquiry.
- **enquiry_Mortgage**: Indicator for a mortgage loan enquiry.
- **enquiry_Real estate loan**: Indicator for a real estate loan enquiry.
- **enquiry_Revolving loans**: Indicator for a revolving loan enquiry.
- **enquiry_Unknown type of loan**: Indicator for an unknown type of loan enquiry.
- **contract_type_Cash loans**: Indicator for having a cash loan contract.
- **contract_type_Revolving loans**: Indicator for having a revolving loan contract.


After conducting a thorough Exploratory Data Analysis (EDA) and Feature Engineering,**feature selection** through **IV(Information Value)** ,out of all engineered features ,
the final dataset consists of the following features:

- **loan_amount**: Total loan amount taken by the borrower.
- **total_loans**: Total number of loans taken by the borrower.
- **active_loan**: Number of active loans.
- **inactive_loan**: Number of inactive loans.
- **amount_overdue**: Amount of the loan that is/was  overdue.
- **avg_overdue_days**: Average number of days overdue for loans.
- **max_overdue_days**: Maximum number of days overdue for loans.
- **total_payments**: Total number of payments made towards loans.
- **avg_loan_duration**: Average duration of loans.
- **number_of_Consumer_credit**: Number of consumer credit loans.
- **number_of_Credit_card**: Number of credit card loans.
- **number_of_Microloan**: Number of microloans.
- **number_of_Mortgage**: Number of mortgage loans.
- **number_of_Car_loan**: Number of car loans.
- **credit_card**: Indicator for having a credit card loan.
- **car_loan**: Indicator for having a car loan.
- **mortgage**: Indicator for having a mortgage loan.
- **microloan**: Indicator for having a microloan.
- **total_enquiry_amount**: Total amount of loan enquiries made.
- **loan_enquiry_ratio**: Ratio of loan enquiries to total loans.
- **overdue_perct**: Percentage of loans that are overdue.
- **contract_type_Cash loans**: Indicator for having a cash loan contract.
- **contract_type_Revolving loans**: Indicator for having a revolving loan contract.

## Models Explored
We have experimented with various machine learning models to predict the loan outcome.
The models explored include:

- **LightGBM**
- **Gradient Boosting**
- **AdaBoost**
- **XGBoost**
- **Decision Tree**
- **Random Forest**
- **Logistic Regression**

## Performed Upsampling,Downsampling and SMOTE(combination of both techniques) as well
## Model Performance: 
The performance of each model was evaluated using ROC- AUC Score as a valid metric.
## Best Performing Model:

#### Based on the evaluation metrics, the best performing model was **Gradient Boosting Classifier**.

## Conclusion
In conclusion, the predictive model developed using the features engineered and various machine learning algorithms can effectively predict the loan outcome for the lending company's applicants.
Further optimizations and fine-tuning or more data can be explored to enhance the model's performance.
