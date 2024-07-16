# Project Title
Prediction of readmission within 30 days based on MIMIC-IV data. This project was conducted during the Data Analytics class in the second semester of 2023.

# Why I do this project?
Readmission is an important issue in the medical field. In particular, the problem of readmission of ICU patients is even more serious. Readmission increases the patient's health risk, increases hospital costs, and reduces patient satisfaction. Therefore, predicting and preventing readmission is important to increase the efficiency of the healthcare system and improve the quality of life of patients. SO, we chose the topic of Prediction of readmission with 30 days.


# Project Process

**Preprocessing**
- If the patient's next visit is less than 30 days, it is converted to 1 and the rest to 0.
- The discharge diagnosis text and readmission column are obtained by combining the admission and discharge data.
- Remove unnecessary parts from the discharge diagnostic text.
- we set the ratio of train, validation, and test sets to 6:2:2. 

**Modeling**
- Pre-trained SapBERT, BlueBERT, bioGPT, bioClinicalBERT models are loaded to proceed with fine tuning.
- The initial learning rate is 3e-5, and the optimizer used is Adam/AdamW.

# Result
+ Modelling results showed that the SapBERT-based model performed best.

![image](https://github.com/user-attachments/assets/1b25dc6b-9ae2-4781-bbbf-7bd3cf30daea)

# contribution
- The model developed in this project can be used to identify patients at high risk of readmission early.
- By predicting the individual patient's risk of readmission, you can develop a customized health care plan.
- Hospitals and healthcare organizations can more efficiently allocate healthcare resources and services based on the predictions of this model.

# Difficult Point
- Setting the topic of readmission prediction with MIMIC-IV (Inserious Care Unit) data.