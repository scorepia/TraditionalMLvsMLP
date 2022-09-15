# TraditionalML vs MLP

## Introduction

งานชิ้นนี้เป็นการเปรียบเทียบศักยภาพในการวิเคราะห์ข้อมูลระหว่าง Traditional Machine Learning (ML) กับ Multilayer Perceptron (MLP) ในข้อมูลประเภท Tabular Data โดยในการเปรียบเทียบครั้งนี้ข้อมูลที่นำมาใช้จะเป็นการจำแนกข้อมูลแบบ Binary Classification 

## Data Source
แหล่งข้อมูล: https://www.kaggle.com/datasets/mastmustu/income

## Environment Setting
  Google Colab with GPU runtimes setting

## Training

ในส่วนของ Traditional Machine Learning ประกอบด้วย Decision Tree, K-Nearest Neighbors, Naive Bayes, Support Vector Machines และ XGboost
ในส่วนของ MLP จะใช้ activation function ใน hidden node คือ relu และ output node คือ sigmoid

## Conclusion

| Model  |  Accuracy (%) | Runtime (s) |
| ----  |  ---- | ---- |
| Decision Tree     |     82.75 | 0.0029
| XGboost     |     86.41 | 2.272
| KNN     |     72.41 | 0.105
| SVM     |     84.13 | 11.907
| Bayes (49 models) | 81.65 | 0.0335 |
| MLP (18 networks)     |     73.87 | 72.3594

จากการทดลองเปรียบเทียบประสิทธิภาพการวิเคราะห์ระหว่าง Traditional ML กับ MLP ในข้อมูลประเภท Tabular Data พบว่า MLP มีค่าเฉลี่ยของ accuracy อยู่ที่ 73.87% และใช้เวลาในการสอนตัวแบบ 72.3594 วินาที ซึ่งเมื่อเทียบกับ ML ที่มี accuracy ที่ใกล้เคียงกัน ได้แก่ KNN ที่มีค่า accuracy อยู่ที่ 72.41% แต่ใช้เวลาในการสอนตัวแบบ 0.105 วินาที หรือ ML ที่ใช้ระยะเวลามากที่สุดคือ SVM ที่มี accuracy อยู่ที่ 84.13% แต่ใช้เวลาในการสอนตัวแบบ 11.907 วินาที จะได้ว่า ML นั้นให้ความแม่นยำที่ใกล้เคียง หรือสูงกว่า MLP โดยที่ใช้ระยะเวลาในการสอนตัวแบบน้อยกว่า และใช้ระยะเวลาในการปรับค่า parameter   ต่าง ๆ น้อยกว่า ทั้งนี้อาจเป็นเพราะชุดข้อมูลที่เลือกใช้ในครั้งนี้มีความซับซ้อนไม่เพียงพอต่อความจำเป็นในการเลือกใช้ MLP

### ปล.รายละเอียดเพิ่มเติมของการทดลองแสดงใน Report

## Member
6310432002 

6410412005

6410412015
