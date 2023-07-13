Overview of the Analysis

Thia Analysis uses financial customer information to determine if a loan is healthy or unhealthy for lending companies.
The data has information about the loan and the borrower, such as the size and the interest rate of the loan, the customer income, debt to income ratio, number of accounts they have, and if they have any derogatory marks.
There is also a data column called loan status which is a binary one using 0 for a healthy loan or 1 for an unhealthy loan. The 0 loans numbered 75036 while the 1 numbered 2500 total.
I performed a split of the customer data into variable X and the binary loan status into variable y. Then used Test Train Split to put the data into a form where we can perform linear regression on it using SkLearn.
After fitting the model and using the Predict Function it was possible to get a classification model that worked satisfactorily. To improve this the data was oversampled as there was very little 1 data as compared to 0 data. After oversampling we performed the same operations.

Results

•	Machine Learning Model 1:

o	Accuracy  0.9218124642767772
o	Precision
	0    1.00
	1     0.85
o	Recall
	0     0.99
	1     0.91

•	Machine Learning Model 2 (resample):

o	Accuracy  0.9205494133884273
o	Precision
	0    0.99
	1    0.99
o	Recall
	0    1.00
	1    0.84

Summary
•	The resampled model was slightly less accurate in terms of balanced accuracy score, but I believe it to be slightly more accurate due to an overall lower spread between the precision and recall values of the 0 and 1
•	It is more important to properly identify the 1 as they represent the unhealthy loans than the 0.
