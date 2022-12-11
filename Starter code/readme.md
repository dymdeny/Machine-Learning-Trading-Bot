## Tune the Baseline Trading Algorithm

In this Challenge, we are assume the role of a financial advisor at one of the top five financial advisory firms in the world. 
I defined the following conditions:

If, the Actual Returns > 0 then system returns Signal value as: 1 (BUY)

If, the Actual Returns < 0 then system returns Signal value as: -1 ( SELL)

I have tested various Models to get the accurate predictions, following are the models I have used with their Performance Summary including "Classification Report" & "Cumulative Return Chart":

**Model 1: PERFORMANCE SUMMARY:**

Following the input parameters:

**Simple Moving Averages (SMA):**
Short Window = 50 Days & Long Window = 100 Days

**Model:**
SVC Classifier

**Classification Report:**

![sma50sma100_classification_report](https://user-images.githubusercontent.com/110307714/206935883-61b39aa4-e731-4867-96f6-25adf243bf47.png)


**Cumulative Return Plot: Actual Returns vs. Strategy Returns**


![svm_model](https://user-images.githubusercontent.com/110307714/206935948-360fd4ac-7013-494d-81c8-a909ae0e99a1.PNG)

**Model:**
Logistic Regression

**Logistic Regression Model Classification Report:**


![lr_sma50_sma100_classification_report](https://user-images.githubusercontent.com/110307714/206935999-202179ae-bf5e-4da5-a799-978fab6b23cd.png)


**Logistic Regression Model Cumulative Return Plot: Actual Returns vs. Strategy Returns**


![logistic_regression_model](https://user-images.githubusercontent.com/110307714/206936027-7a1c7829-03a7-444c-b1ed-2f2a471c6c1b.PNG)


**Model 2:PERFORMANCE SUMMARY:**

Following the input parameters:

**Simple Moving Averages (SMA):**
Short Window = 8 Days & Long Window = 50 Days

**Model:**
SVC Classifier

**Classification Report:**

![sma8_Sma50_classification_report](https://user-images.githubusercontent.com/110307714/206936103-7845efc5-0f2a-47fb-8cb3-0d8c4ad72e8a.png)

**Cumulative Return Plot: Actual Returns vs. Strategy Returns**

![svm_model_sma8_sma50](https://user-images.githubusercontent.com/110307714/206936160-bffcff2e-4cbc-4d86-9879-141415dc0fe7.PNG)


**Model:**
LogisticRegression

**Logistic Regression Model Classification Report:**

![lr_model_sma8_sma50_classification report](https://user-images.githubusercontent.com/110307714/206936196-012d4f3d-2404-464f-bab0-963d5c8a3d2d.png)


**Logistic Regression Model Cumulative Return Plot: Actual Returns vs.  Strategy Returns**

![logistic_regression_model_sma8_sma50](https://user-images.githubusercontent.com/110307714/206936207-36ece23d-8f43-4cc2-ac72-9420ede179cc.PNG)



**Model 3:  PERFORMANCE SUMMARY:**

Following  the input parameters:

**Simple Moving Averages (SMA):**
Short Window = 100 Days & Long Window = 200 Days

**Model:**
SVC Classifier

**Classification Report:**


![sma100_sma200_classification_report](https://user-images.githubusercontent.com/110307714/206936300-b5211638-cf06-4cc3-9e68-148f1916f67e.png)



**Cumulative Return Plot: Actual Returns vs. Strategy Returns**


![svm_model_sma100_sma200](https://user-images.githubusercontent.com/110307714/206936314-e3ed826d-0b8b-4e7a-9403-24313188ffec.PNG)


**Model:**
LogisticRegression

**Logistic Regression Model Classification Report:**

![lr_model_sma100_sma200_classification report](https://user-images.githubusercontent.com/110307714/206936350-2fe54a69-64d0-46cf-b2fb-6e94dff078b2.png)

**Logistic Regression Model Cumulative Return Plot: Actual Returns vs. Strategy Returns**

![logistic_regression_model sma100_sma200](https://user-images.githubusercontent.com/110307714/206936362-a749600b-9c25-48b2-b534-88083966f918.PNG)


**Results:**

In conclusion,Classification Reports & Cumulative Returns Graphs of the second model with input parameters of short window = 8 and long window = 50 showing the best results. Both SVC Classifier and LogisticRegression Model showing decent improvment in return curve and accuracy score respectively. Based on information provided above, I can say that, decreasing SMA short and long window can improve algorithm trading model performance. 
