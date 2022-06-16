# Logistic-Regression---Titanic-Dataset
Titanic dataset is one of the datasets available in sklearn.
In the training data we have missings in the age, cabin and embarked column. In the test data set are missings in the age, fare and cabin column. We will concat both data sets and perform the data cleansing for the entire data set.

## DATA CLEANING
### 1. AGE
![WhatsApp Image 2022-06-14 at 7 25 51 PM](https://user-images.githubusercontent.com/98227015/173594970-ac3fe587-19d9-47f4-b46a-4d7f5308d873.jpeg)

We don´t want to delete all rows with missing age values, therefore we will replace the missings. As you can see we have a right-skrewed distribution for age and the median should a good choice for substitution.

One thesis was that the median of age differs for the passenger classes. Professional advancement usually comes with increasing age and experience. Therefore, people with a higher socio-economic status are older on average. If we split up by sex we see that there is still a difference because women are younger in general. In a last step I have checked the number of cases to ensure that there are still enough cases in each category. We will use these median values to replace the missings.

### 2.FARE
![WhatsApp Image 2022-06-14 at 7 28 21 PM](https://user-images.githubusercontent.com/98227015/173595424-6b244ed4-9efb-4a1e-a312-eb3677f31e55.jpeg)

### 3.CABIN 
There are a lot of missing values but we should use the cabin variable because it can be an important predictor. As you can see in the following picture, the first class had the cabins on deck A, B or C, a mix of it was on D or E and the third class was mainly on f or g. We can identify the deck by the first letter.

![WhatsApp Image 2022-06-14 at 7 35 55 PM](https://user-images.githubusercontent.com/98227015/173597148-8eaea7d6-4323-438a-80f7-51f566ea7479.jpeg)

