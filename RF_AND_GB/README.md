[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/tX8-4Blr)
# Задача классификации (домашнее задание 3).

Необходимо научиться предсказывать преддиабетное состояние или диабет по результатам анализов и опрососа.

**Target:** Diabetes_binary - 0 = no diabetes 1 = prediabetes or diabetes  
**Features:**  
1. HighBP - 0 = no high BP, 1 = high BP
2. HighChol - 0 = no high cholesterol, 1 = high cholesterol
3. holCheck 0 = no cholesterol check in 5 years, 1 = yes cholesterol check in 5 years
4. BMI - Body Mass Index
5. Smoker - Have you smoked at least 100 cigarettes in your entire life? (Note: 5 packs = 100 cigarettes) 0 = no, 1 = yes
6. Stroke (Ever told) you had a stroke. 0 = no, 1 = yes
7. HeartDiseaseorAttack - coronary heart disease (CHD) or myocardial infarction (MI) 0 = no, 1 = yes
8. PhysActivity - physical activity in past 30 days - not including job 0 = no, 1 = yes
9. Fruits - Consume Fruit 1 or more times per day 0 = no, 1 = yes
10. Veggies - Consume Vegetables 1 or more times per day 0 = no, 1 = yes
11. HvyAlcoholConsump - (adult men >=14 drinks per week and adult women>=7 drinks per week) 0 = no, 1 = yes
12. AnyHealthcare - Have any kind of health care coverage, including health insurance, prepaid plans such as HMO, etc. 0 = no 1 = yes
13. NoDocbcCost - Was there a time in the past 12 months when you needed to see a doctor but could not because of cost? 0 = no 1 = yes
14. GenHlth - Would you say that in general your health is: scale 1-5 1 = excellent 2 = very good 3 = good 4 = fair 5 = poor
15. MentHlth - days of poor mental health scale 1-30 days
16. PhysHlth - physical illness or injury days in past 30 days scale 1-30
17. DiffWalk - Do you have serious difficulty walking or climbing stairs? 0 = no 1 = yes
18. Sex - 0 = female 1 = male
19. Age - 13-level age category 1 = 18-24 .. 9 = 60-64, 13 = 80 or older
20. Education - Education level (EDUCA see codebook) scale 1-6 1 = Never attended school or only kindergarten 2 = elementary etc.
21. Income - Income scale  scale 1-8: 1 = less than 10,000 usd ... 5 = less than 35,000 usd ... 8 = 75,000 usd or more

**Метрика должна быть нацелена на выявление диабета, при этом штрафовать за пропущенный диабет в два раза больше, чем за ошибочный диагноз диабета.**

В вашем итоговом файле должны быть собраны **три модели** и получено три оценки (три вектора y_pred_...). Важно соблюдать требования по оформлению имен данных векторов, или оценка будет снижена.  
Алгоритмы оцениваемые:
1. Оценка полученная на основе алгоритма  `RandomForestClassifier` или `ExtraTreesClassifier`
2. Оценка полученная на основе алгоритма  `GradientBoostingClassifier` или `HistGradientBoostingClassifier`
3. Оценка итоговой модели. Тут может быть любая модель из `scikit-learn` за исключением нейросетей. Естественно можно использовать `Voiting` или `Staking`.
