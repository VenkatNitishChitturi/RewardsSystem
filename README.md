# RewardsSystem
This project is a restful service build using spring boot to track rewards for customers.

Instructions on how to use:

1) Import this project by git clone command into your local machine.
2) Open the project directory that has the pom.xml into a IDE like IntelliJ or Eclipse.
3) The Spring boot application can be run by running the main java file - RewardsApplication.java
4) After the spring boot application is running go to a local browser and enter - http://localhost:8080/ to check if it is running as expected.
5) It should show the message: Hello Welcome to rewards calculator!
6) Now enter in the browser: http://localhost:8080/getCustomer/customer1 to get the details fo the customer including: 
customerId, firstname, lastname, phoneNumber, email and transactions. Transactions is again a list of transaction each including: 
id, itemName, amount, date, customerId
8) Now enter in the browser: http://localhost:8080/getCustomerRewardSummary/customer1 to get the rewards summary of customer 1 based on the data files given as sample in the project under resources - "customer_data.txt" and "transaction_data.txt".
9) This data files contain customer data and their transactions(for three months period) in two separate files.
10) It should show the output consisting of :
customer id, totalRewardPoints, rewardPointsPerMonth which is a list of rewardsPoints each including:
month, points
Example for customer 1: {"customerId":"customer1","totalRewardPoints":210,"rewardPointsPerMonth":{"6":180,"7":10,"8":20}}
9) Repeat the same to check for customer2, customer3 and customer4. 
10) To test more you can modify the data files mentioned under point 6 to get different data.


