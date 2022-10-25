# Predicting-User-Adoption
This project used ML to identify which factors predict future user adoption of an online service.

This was a mock take home assessment, with data and business case prompt provided.


## **Approach:** Adopted users were defined and labeled in the users table based on entries in the logins table. I derived some additional features, including the number of users in an organization and how many were active, whether a user was invited by an active user, and whether a user had invited other users and whether or not they were active. I fit the scaled & encoded data to an XGBoosted Tree Classifier and then found the SHAP values associated with each feature. SHAP values are plotted below for review.





### **Factors which predict future user adoption, in order of importance:**
1. Belonging to an organization with a higher percentage of adopted users
2. Being invited by an adopted user
3. Having an @hotmail.com email address
4. Signing up through Google Authentication or through a guest invite
5. Being opted in to the mailing list
6. Having a @gmail.com email address


### **Factors which were found to predict a user not becoming adopted:**
1. Creating an account for personal projects
2. Having an @yahoo.com email address
3. Having a higher number of users in their organization
4. Being invited through their organization



