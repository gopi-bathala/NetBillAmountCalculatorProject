# NetBillAmountCalculatorProject
This service is used to calculate the final bill amount by applying necessary discounts

## Reference Documentation

### 1. Executing the service

Please follow below steps for executing this service directly in windows operating system.

Step 1: Please download "NetPayCalcService-0.0.1-SNAPSHOT.jar" under /target folder from GitHub and save it under "D:\" path.

Step 2: Open Command Prompt and execute below mentioned script.

	java -jar D:\NetPayCalcService-0.0.1-SNAPSHOT.jar

Step 3: After successful start up, you will see below message under Command Prompt Console.

	Started NetPayCalcServiceApplication in XX seconds

### 2. Testing the service

Please find below URI Details:

	URI : http://localhost:8080/calculateNetBillAmt/{billAmt}/{customerType}/{purchaseType}
	
Please change below parameter values: 
	
	{billAmt} : This parameter will hold the initial bill amount before applying the discount. Please follow format like 10000.00
	
	{customerType}: This parameter will hold the customer Type value. The possible values are Employee , Affiliate, LoyalCustomer , Others
	
	{purchaseType}: This parameter will hold the purchase type value. The possible values are Groceries, Others.
	
Below example URL:
	
	http://localhost:8080/calculateNetBillAmt/1000/LoyalCustomer/Groceries
	
Sample Response:

	{"finalBillAmt":1000.0,"errorCode":"000","errorDesc":"Success"}
			
I have also prepared Swagger API documentation for this service where we can view request and response as well. Please hit below URL to view complete swagger API documentation.
	
	http://localhost:8080/swagger-ui.html
	
### 3. Code Coverage

I have used jacoco plugin for generating code coverage reports. Please find the coverage report using below html file.

	/NetPayCalcService/target/site/jacoco/index.html
  
 ### 4. JUnit Test Cases
 
I have done unit testing. These test cases are available under below file. Please check
  
  	/src/test/java/com.gopi.NetPayCalcServiceApplicationTests.java
  
### 5. UML Diagram

I have created class diagram and kept the same under below file for your reference. Please check

	NetPayCalcClassDiagram.ucls
  
### 6. Conclusion

I hope this document provides sufficient information about the service. Please contact me in case of further queries.

Awaiting positive response. Thank you. 

	Gopi Bathala
	0544069844
	gopinath524@gmail.com

