# Predicting-User-Adoption
## Task: 
This was a take-home assessment from psuedo-company "Relax, Inc."
Defining an "adopted user" as a user who has logged into the product on three separate days in at least one seven­day period, my task was to identify which factors predict future user adoption.

## Data: 
Two .csv files containing the following information:
1. A user table with data on 12,000 users who signed up for the product in the past 2 years
2. A usage summary table with a row for each day that a user logged into the product

## **Approach:**
Adopted users were defined and labeled in the users table based on entries in the logins table. I derived some additional features, including the number of users in an organization, how many organization users were active, whether a user was invited by an active user, how many invitations a user had sent to others who signed up, and how many of their invitees were now adopted users. I fit the scaled & encoded data to an XGBoosted Tree Classifier and then found the SHAP values associated with each feature to interpret their influence on the results. SHAP values are plotted below for review.

[img](https://github.com/caitlinruble/Predicting-User-Adoption/blob/0f6f2a854427450c18f4c75c9bb1149332c30896/Model%20SHAP%20values.png)

## **Results:**


### **Factors which predict future user adoption, in order of importance:**
1. Belonging to an organization with a higher percentage of adopted users
2. Being invited by an adopted user
3. Having an @hotmail.com email address
4. Signing up through Google Authentication or through a guest invite
5. Being opted in to the mailing list
6. Having a @gmail.com email address


### **Factors which were found to predict a user *not* becoming adopted:**
1. Creating an account for personal projects
2. Having an @yahoo.com email address
3. Having a higher number of users in their organization
4. Being invited through their organization



