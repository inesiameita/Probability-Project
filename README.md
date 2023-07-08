# Data Analysis of Customer Vehicle Insurance - Probability Project

# Introduction
Insurance policies provide compensation for specific losses or damages in exchange for regular premium payments. This project analyzes a dataset of vehicle insurance to explore the probabilistic relationships between various factors. The dataset includes information on demographics, vehicles, and insurance policies, such as gender, age, region code type, vehicle age, damage, premium, and sourcing channel. The goal is to gain insights into the factors that influence vehicle insurance and understand the probabilistic relationships between these variables. By examining these relationships, businesses can make informed decisions and optimize their strategies in the vehicle insurance industry.

# Dataset Overview
The dataset used in this project is obtained from Kaggle’s “Health Insurance Cross Sell Prediction” dataset. It contains several variables, including:
- id : Unique ID for the customer
- Gender : Gender of the customer
- Age : Age of the customer
- Driving_License 
    0 : Customer does not have DL, 
    1 : Customer already has DL
- Region_Code : Unique code for the region of the customer
- Previously_Insured 
    1 : Customer already has Vehicle Insurance, 
    0 : Customer doesn't have Vehicle Insurance
- Vehicle_Age : Age of the Vehicle
- Vehicle_Damage 
    1 : Customer got his/her vehicle damaged in the past. 
    0 : Customer didn't get his/her vehicle damaged in the past.
- Annual_Premium : The amount customer needs to pay as premium in the year
- Policy_Sales_Channel : Anonymized Code for the channel of outreaching to the customer ie. Different Agents, Over Mail, Over Phone, In Person, etc.
- Vintage : Number of Days, Customer has been associated with the company
- Response 
    1 : Customer is interested, 
    0 : Customer is not interested

# Research Questions
The purpose of this analysis is to gain deeper insights and understanding of vehicle insurance data. The project involves conducting various analyses using Python libraries. Before proceeding with the analysis, the dataset is imported and necessary libraries are imported as well. This ensures that the dataset is prepared for further exploration and analysis.
![image](https://github.com/inesiameita/Probability-Project/assets/128911434/909c68e3-bfea-473f-8727-f0e59697d286)

The dataset has been successfully imported using the "pd.read_csv" function. By displaying the dataset information, including column names, data types, and the number of non-null values in each column, we gain an overview of the dataset. This step allows us to understand the structure and characteristics of the data before further analysis.
![image](https://github.com/inesiameita/Probability-Project/assets/128911434/d6ed341f-6b97-4613-9323-18d780e4c161)

Next, we identify NaN values and we identify if there are any duplicate data in the dataset we are using the following approach:
![image](https://github.com/inesiameita/Probability-Project/assets/128911434/1111bf5d-40b6-49a5-ba44-8654b8a48dc1)

![image](https://github.com/inesiameita/Probability-Project/assets/128911434/9bc514c3-803a-4f4a-a300-fb39271f6a44)


After data processing has been performed and the data quality has been ensured for analysis, we can proceed with the data analysis process.

# Descriptive Statistical Analysis
Question 1 : What is the average age in this data?

![image](https://github.com/inesiameita/Probability-Project/assets/128911434/acdde26a-9ede-440a-b5f3-3ce2938601a9)


Question 2 : What is the average premium that customers need to pay in a year?

![image](https://github.com/inesiameita/Probability-Project/assets/128911434/5834992e-be16-4e33-94bf-04957a0ad053)


Question 3 : What is the total number of male customers and female customers?

![image](https://github.com/inesiameita/Probability-Project/assets/128911434/4ffc7a08-330c-4b0d-a139-da2ad1c859ab)


Question 4 : What is the average age of male and female customers?

![image](https://github.com/inesiameita/Probability-Project/assets/128911434/e093623e-3f12-44cd-978a-9c1566dbb42a)


Question 5 : What is the average annual premium paid by customers who have vehicle insurance and those who do not have vehicle insurance?

![image](https://github.com/inesiameita/Probability-Project/assets/128911434/bbe67303-b067-4939-9a6c-e14f0b189225)


Question 6 : What is the average annual premium paid by customers who have driving license and those who do not have driving license?

![image](https://github.com/inesiameita/Probability-Project/assets/128911434/289a07d6-4b8e-4f9c-a2b6-1546a062c60d)


Question 7 : What is the variance of the annual premiums paid by customers who have vehicle insurance and those who do not have vehicle insurance?

![image](https://github.com/inesiameita/Probability-Project/assets/128911434/6fc60e6f-aa0b-49fa-82fe-67689926481c)

# Discrete Variable Analysis
Question 1 : How is probability mass function distribution of the customer age?

![image](https://github.com/inesiameita/Probability-Project/assets/128911434/9f711f63-1668-4de1-82ab-40e2c0aa50ad)

The resulting plot will show the probability distribution of the customer age in the dataset.


Question 2 : What is the proportion of the number of male vs female customers? Which gender has the higher proportion?

![image](https://github.com/inesiameita/Probability-Project/assets/128911434/c169906b-f4f5-4e71-a5d6-02973e385d86)

Based on the table and graph above, it is evident that the proportion of male customers is higher than that of female customers, with a proportion of 0.540761.


Question 3 : What is the proportion of the average annual premium of male vs female customers?

![image](https://github.com/inesiameita/Probability-Project/assets/128911434/49bbaac6-f2fd-4c1b-99c1-66daeb654748)

Based on the table and graph above, it is evident that the average annual premium for male customers is slightly higher than that for female customers, with a proportion of 0.501038. However, the difference in values between the two proportions is not significant.


Question 4 : What is the proportion of the number of customer who have vehicle insurance vs customer who do not have vehicle insurance?

![image](https://github.com/inesiameita/Probability-Project/assets/128911434/cfc9c3df-bee7-490f-88cd-d5919f4a298e)

Based on the table and graph above, it is evident that the proportion of customers who have vehicle insurance is smaller than the proportion of customers who do not have vehicle insurance, with a proportion of 0.45821.


Question 5 : What is the proportion of the number of customer’s vehicle age?

![image](https://github.com/inesiameita/Probability-Project/assets/128911434/f0f2cfb2-a351-466e-b8e3-f52a587eca92)

Based on the table and graph above, it is evident that the proportion of customers based on the age of their vehicles varies. The category of vehicles with an age of 1–2 years has the highest proportion, which is 0.525613, compared to the other categories. On the other hand, the category of vehicles with an age of more than 2 years has the smallest proportion, which is 0.042001.


Question 6 : What is the proportion of the number of customer’s response?

![image](https://github.com/inesiameita/Probability-Project/assets/128911434/845dcfb7-5c3f-4b89-a298-4efe1b2a8ce1)

Based on the table and graph above, it is evident that the proportion of customers interested in having vehicle insurance is smaller than the proportion of customers who are not interested, with a proportion of 0.877437.


Question 7 : What is the probability of customers being interested in having insurance when the age of their vehicle is less than 1 year?

![image](https://github.com/inesiameita/Probability-Project/assets/128911434/fd020666-ea22-44cd-bf76-f2288b0ca92e)

The probability of customers being interested in having insurance when the age of their vehicle is less than 1 year : 0.018898.


Question 8 : What is the probability of customers being interested in having insurance when the customer ever had previously insurance?

![image](https://github.com/inesiameita/Probability-Project/assets/128911434/c7f3ac2d-3362-406b-af86-b326381d1f5d)

The probability of customers being interested in having insurance when the customer ever had previously insurace : 0.00041458.


# Continuous Variable Analysis
Question 1 : Which one is more likely to occur
- Customer above the age of 30 pays annual premium above 30500
- Customer below the age of 30 pays annual premium above 30500

![image](https://github.com/inesiameita/Probability-Project/assets/128911434/ea548fee-a6a3-4545-b616-e910ea98ddad)


Question 2 : Which one is more likely to occur
- Customer above the age of 30 who have previous insurance
- Customer below the age of 30 who have previous insurance

![image](https://github.com/inesiameita/Probability-Project/assets/128911434/cfbaf3f2-c58d-4179-9a6a-5fd3ed2c8259)


Question 3 : Which one is more likely to occur
- Customer above the age of 30 who do not have previous insurance and pays annual premium above 30500
- Customer below the age of 30 who have previous insurance and pays annual premium above 30500

![image](https://github.com/inesiameita/Probability-Project/assets/128911434/12410d11-f962-4948-a305-2fbd5a4b5d12)


# Variable Correlation Analysis
Question 1 : How is the correlation between the variables Age and Annual Premium?

![image](https://github.com/inesiameita/Probability-Project/assets/128911434/ca12bf59-03bb-4c3c-9fa9-1bfbd9b08f11)

The correlation age and annual premium at customer have insurance is 0.06750700155668837
Based on the plot, it can be observed that the correlation between age with annual premium is positive, but the correlation is weak with a value of 0.06751. This indicates that the variables age have a positive influence, but it is not really significant on annual premium.

Question 2 : How is the correlation between the variables Previously_Insured = 1, Age and Annual Premium?

![image](https://github.com/inesiameita/Probability-Project/assets/128911434/4d4097b1-df1b-4ba0-a2da-427635304f42)

The corelation age and customer have insurance at annual premium is 0.02687233319314686
Based on the plot, it can be observed that the correlation between age where the previously insured is yes with annual premium is positive, but the correlation is weak with a value of 0.02687. This indicates that the variables age and previously insured have a positive influence, but it is not really significant on annual premium.

Question 3 : How is the correlation between the variables Response = 1, Age and Annual Premium?

![image](https://github.com/inesiameita/Probability-Project/assets/128911434/61d7dc61-6d82-41bd-96cc-e80a497fe538)

The corelation age where the customer have interest in insurance at annual premium is 0.12395984204766056
Based on the plot, it can be observed that the correlation between age where the customer have interest in insurance with annual premium is positive, but the correlation is weak with a value of 0.12396. This indicates that the variables age and response have a positive influence, but it is not really significant on annual premium.

Question 4 : How is the correlation between the variables Vehicle Age below 1, Age and Annual Premium?

![image](https://github.com/inesiameita/Probability-Project/assets/128911434/db0c6a0a-1a3a-45b8-a4e6-984206f43b4b)

The corelation age and annual premium at customer have insurance is -0.08218165200944164
Based on the plot, it can be observed that the correlation between age where the vehicle age below 1 year with annual premium is negative, but the correlation is weak with a value of -0.08218. This indicates that the variables age and vehicle age below 1 year have a negative influence, but it is not really significant on annual premium.

# Hypothesis Testing
Question 1 : The annual premium for those previously insured is less than or equal to the annual premium for those not previously insured
H0 = Annual premium have previously insured <= annual premium not have previously insured
H1 = Annual premium have previously insured > annual premium not have previously insured

![image](https://github.com/inesiameita/Probability-Project/assets/128911434/4a71b805-f5c2-4a96-8876-32e621f55703)

From the above result, it is known that the p-value is 0.00382, therefore H0 is rejected. This means that there is enough evidence to conclude that there is a significant difference between the tested groups, indicating that the Annual Premium for those who have previously insured is greater than the annual premium for those who have not previously insured.

Question 2 : The annual premium have driven license is less than annual premium not have driven license
H0 = Annual premium have driven license <= annual premium not have driven license
H1 = Annual premium have driven license > annual premium not have driven license

![image](https://github.com/inesiameita/Probability-Project/assets/128911434/b17da756-11df-4680-bf8c-59a8206885a8)

From the above result, it is known that the p-value is 0.9999999999920179, we fail to reject H0. This means that there is not enough evidence to conclude the presence of a significant difference between the tested groups. In this context, we cannot draw the conclusion that the alternative hypothesis H1 is true or that a significant difference exists between the tested groups, indicating that the Annual Premium for those who have have driven license is less than or equal to the annual premium for those who have not driven license.

Question 3 : The proportion of license-driven owners with response 1 is greater than or equal to the proportion of non-license-driven owners with response 1
H0 = Proportion of license-driven owners with response 1 >= proportion of non-license-driven owners with response 1
H1 = Proportion of license-driven owners with response 1 < proportion of non-license-driven owners with response 1

![image](https://github.com/inesiameita/Probability-Project/assets/128911434/14347f63-965c-44ac-ad56-2e967269b6ee)

From the above result, it is known that the p-value is 0.0.9999999998185439, we fail to reject H0. This means that there is not enough evidence to conclude the presence of a significant difference between the tested groups. In this context, we cannot draw the conclusion that the alternative hypothesis H1 is true or that a significant difference exists between the tested groups, indicating that the proportion of license-driven owners with interested in having insurance is greater than or equal to proportion of non-license-driven owners with interested in having insurance.

Question 4 : The proportion of previous insurance owners with response 1 is greater than or equal to the proportion of insurance owners with response 0
H0 = Proportion of previous insurance owners with response 1 >= proportion of insurance owners with response 0
H1 = Proportion of previous insurance owners with response 1 < proportion of insurance owners with response 0

![image](https://github.com/inesiameita/Probability-Project/assets/128911434/c03e7f42-7921-4f9f-8058-ac00323828bc)

From the above result, it is known that the p-value is 0.0. Therefore, we reject H0 and accept the alternative hypothesis H1, suggesting that there is a significant difference or relationship between the variables being tested. Proportion of previous insurance owners with response 1 is less than proportion of insurance owners with response 0.

Question 5 : The variance of annual premium for males and females is the same
H0 = variance annual premium for males = variance annual premium females
H1 = variance annual premium for males ≠ variance annual premium females

![image](https://github.com/inesiameita/Probability-Project/assets/128911434/e9f1a86f-5620-40f4-9b52-4a60ebdae59e)

From the above result, it is known that the p-value is 5.114293745910101e-65, we can conclude that the result is statistically significant. The extremely small pvalue indicates that the observed data is highly unlikely to occur under the assumption of equal variances between the groups being compared. Therefore, we reject H0 and accept the alternative hypothesis H1, indicating that there is a significant difference in the variances between annual premium for males and annual premium females.


# Summary and Conclusion
1. Descriptive statistical analysis provided insights into customer characteristics, such as average age, average annual premiums,   gender proportions, and the proportion of customers with vehicle insurance.
2. Discrete and continuous variable analyses explored probabilistic relationships between variables, including the probability mass function distribution of customer age, gender proportions, average annual premiums by gender, proportions of customers with vehicle insurance, proportions based on vehicle age, and proportions of customer interest in insurance.
3. Variable correlations and hypothesis testing helped understand the relationships between age, annual premiums, and other variables, determining significant relationships and differences between groups. These analyses contribute to informed decision-making, optimization of communication strategies, and improvement of the overall business model and revenue in the vehicle insurance industry.

In conclusion, this analysis provided valuable insights into the vehicle insurance dataset, offering understanding of customer characteristics, preferences, and relationships between variables. The findings can support informed decision-making, optimization of communication strategies, and improvement of the overall business model and revenue.


