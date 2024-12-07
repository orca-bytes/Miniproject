# Miniproject
#Data180 Group MiniProject
#Group Mini Project

#Summary statistics table and data cleaning steps including: missing values (if any); transformations of the data (if required, such as normalizing or converting to factor variables); a narrative of which variables you think make sense as predictors for default


library(readxl)
mini_data = read_excel("~/Documents/INFO180/GROUP MINI PROJECT/default of credit card clients.xls", skip = 1)
summary(mini_data)
mini_data$SEX = factor(mini_data$SEX)
mini_data$EDUCATION = factor(mini_data$EDUCATION)
mini_data$MARRIAGE = factor(mini_data$MARRIAGE)
mini_data$PAY_0 = factor(mini_data$PAY_0)
mini_data$PAY_2 = factor(mini_data$PAY_2)
mini_data$PAY_3 = factor(mini_data$PAY_3)
mini_data$PAY_4 = factor(mini_data$PAY_4)
mini_data$PAY_5 = factor(mini_data$PAY_5)
mini_data$PAY_6 = factor(mini_data$PAY_6)

#I AM PREDICTING THAT "PAY_0,1,2,3,4... PAY_6" ARE EXPECTED TO BE SIGNIFIGANT PREDICTORS FOR CLIENT RISK OF DEFAULT.


