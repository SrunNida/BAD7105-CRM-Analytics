# Customer Response model

I had done training the model both using low-level libraries like sklearn and high-level library (Pycaret)

But I will explain only the part that using Pycaret

![image](https://user-images.githubusercontent.com/88968324/146376726-64da654e-7ddd-4de5-b603-af8dc8acb01f.png)

Others than customer_id column, there were features that I used for model, and response column is label

![image](https://user-images.githubusercontent.com/88968324/146377021-61391337-5f2f-4f23-946c-87750eeabfc0.png)

From bar chart, you can see that data really imbalance (0 as not response, 1 as response)

![image](https://user-images.githubusercontent.com/88968324/146377229-1daa9919-53da-49bf-80ef-6c9433c715e1.png)

Put data into Pycaret classification

As you can see, I normalized data using zscore and fix imbalance using SMOTE (Over sampling method)

** Ignor customer_id

![image](https://user-images.githubusercontent.com/88968324/146377401-5877b13e-afc3-48cf-878e-aa418ecbf839.png)
![image](https://user-images.githubusercontent.com/88968324/146377428-4e8fec26-ffab-480f-a147-9523c29f6dda.png)

Data split train and test set as 80%:20%, and did 10 fold cross validation

![image](https://user-images.githubusercontent.com/88968324/146377536-ba510fbf-5ccf-4ee2-80bb-a069400f9c36.png)

Before tuning, the best AUC-score model was lightgbm as 0.70

![image](https://user-images.githubusercontent.com/88968324/146377689-0d759683-8757-43b9-96d2-a7fc02a2c838.png)

After tuning hyperparameter for lightgbm, AUC increased from 0.7 to 0.77, but Accuracy decreased from 0.87 to 0.66

So model before tuning is more reliable.

![image](https://user-images.githubusercontent.com/88968324/146378263-8b7065d2-c1e6-437b-a723-0c24ff7863a3.png)

ROC curves

![image](https://user-images.githubusercontent.com/88968324/146378303-c45a5685-2ad3-41bd-8c2b-d0b4c408f2ec.png)

Confusion matrix

![image](https://user-images.githubusercontent.com/88968324/146378426-2fcd57e4-d502-492e-a8e6-679b8bbb4c7d.png)

Important features

![image](https://user-images.githubusercontent.com/88968324/146378485-4b2f77fe-185e-4ee3-a340-500e878a030a.png)
