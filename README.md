# absent

Absentism at work

Introduction

Absenteeism is an employee's intentional or habitual absence from work. While employers expect workers to miss a certain number of workdays each year, excessive absences can equate to decreased productivity and can have a major effect on company ​nances, morale and other factors.
Habitual non-presence extends beyond what is expected as a normal amount of time away for reasons such as scheduled vacation or occasional illness. Possible causes of absen- teeism include job dissatisfaction, ongoing personal issues and chronic medical problems. Regardless of the cause, a worker with a pattern of being absent may put his reputation and his employed status at risk. Poor attendance by employees becomes a burden on the company and the rest of the staff. Because of the drop in productivity their absence causes and the extra work handed to other staff members which impact morale, they are a financial burden to the organization.
Employees who are frequently absent from the job prevent their team members from being productive. Rather than having the team member complete his task during regular work hours, the team may have to either extend their work hours or even work on weekends all this to adjust to certain employees not being available at work. Temporary replacements of team members due to the absenteeism of the core team member makes it extremely diffcult for a manager to determine the skill set and how that employee its into the workof the group.
In every organization, there are these employees who are allowed to continue an ex- cessive number of absences without any penalty from the senior leadership this partiality can hurt others performance. This leads to low productivity, poor employee morale, and a high attrition rate.
The employee is expected to develop professionally as the organization grows. When that employee has poor attendance, his performance gets affected and he is no longer able to add value to the company in helping to fulfill the arms growth objectives. Team members who are left to cover for employees with poor attendance records eventually start to dislike their chronic absenteeism. Over time, this frustration can result in open conflict between staff members which will not be in the best interest of the organization.

Methodology
Data Retrieval and Cleaning
 
  In this project, the dataset Absenteeism at Work has been used to predict the probability of a person being absent to work. The dataset has been accessed from [1]. There are a total of 20 features in the dataset. The features are :
1. Reason for absence : This attribute gives information of the reason for the em- ployee's absence. The data column had values ranging from 1 to 28. The categories are as follows
Absences attested by the International Code of Diseases (ICD) stratified into 21 categories(1 to 21) as follows :
1 : Certain infectious and parasitic diseases
2 : Neoplasms
3 : Diseases of the blood and blood-forming organs and certain disorders involving the immune mechanism
4 : Endocrine, nutritional and metabolic diseases
5 : Mental and behavioural disorders
6 : Diseases of the nervous system
7 : Diseases of the eye and adnexa
8 : Diseases of the ear and mastoid process
9 : Diseases of the circulatory system
10 : Diseases of the respiratory system
11 : Diseases of the digestive system
12 : Diseases of the skin and subcutaneous tissue
13 : Diseases of the musculoskeletal system and connective tissue
14 : Diseases of the genitourinary system
15 : Pregnancy, childbirth and the puerperium
16 : Certain conditions originating in the perinatal period
17 : Congenital malformations, deformations and chromosomal abnormalities
18 : Symptoms, signs and abnormal clinical and laboratory findings, not elsewhere classified
19 : Injury, poisoning and certain other consequences of external causes
20 : External causes of morbidity and mortality
21 : Factors influencing health status and contact with health servicesand the 7 categories without (CID) are :
22 : patient follow-up
23 : Medical consultation
24 : Blood Donation
25 : Laboratory examination
26 : Unjustified absence
27 : Physiotherapy
28 : Dental consultation
All the above mentioned values ranging from 1 to 28 are valid for reasons of absence. No impossible values have been observed in the data column.
2. Month of absence : This attribute gives information of the month in which the employee was absent. The data column had values ranging from 0 to 12. These values are made more sensible by assigning a category which is meaningful in the real world. Below are the categories mentioned :
1 replaced with January
2 replaced with February 3 replaced with March
4 replaced with April
5 replaced with May
6 replaced with June
7 replaced with July
8 replaced with August
9 replaced with September
10 replaced with October
11 replaced with November
12 replaced with December
All the above mentioned values ranging from 1 to 12 are valid months. An im- possible value of "0" was observed, which does not co-relate to any month in the real world. The dataset contains 3 observations with this value, and all have been removed to make the dataset more meaningful.
3. Day of the week : This attribute gives information of the day of the week on which the employee was absent. The data column had values ranging from 2 to 6. These values are made more sensible by assigning a category which is meaningful in the real world. Below are the categories mentioned :
2 replaced with Monday
3 replaced with Tuesday
4 replaced with Wednesday
5 replaced with Thursday
6 replaced with Friday
All the above mentioned values ranging from 2 to 6 are valid days of the week. No impossible values have been observed in the data column.
4. Seasons : This attribute gives information of the season in which the employee was absent. The data column had values
 
 
ranging from 1 to 4. These values are made more sensible by assigning a category which is meaningful in the real world. Below are the categories mentioned :
1 replaced with Summer
2 replaced with Autumn
3 replaced with Winter
4 replaced with Spring
All the above mentioned values ranging from 1 to 4 are valid seasons. No impossible values have been observed in the data column.
5. Transportation expense : This attribute gives information of the Transport cost for the employee to and fro work each day. The data column had values ranging from 118 Brazilian Real to 388 Brazilian Real. No impossible values have been observed in the data column.
6. Distance from residence to work : This attribute gives information of the Distance in kilometers for the employee to work. The data column had values ranging from 5 kilometers to 52 kilometers. No impossible values have been observed in the data column.
7. Service time : This attribute gives information of the number of years in service the employee has dedicated to the company. The data column had values ranging from 1 year to 29 years. No impossible values have been observed in the data column.
8. Age : This attribute gives information of the age of the employee. The data column had values ranging from 27 years to 58 years. No impossible values have been observed in the data column.
9. Work load Average/day : This attribute gives information of the average work load per day. The data column had values ranging from 205917 to 378884. No impossible values have been observed in the data column.
10. Hit target : This attribute gives information of the percent of targets hit by the employee. The data column had values ranging from 81% to 100%. No impossible values have been observed in the data column.
11. Disciplinary failure : This attribute gives information whether the employee has faced any disciplinary action or no. The data column had values of 0 and 1. These values are made more sensible by assigning a category which is meaningful in the real world. Below are the categories mentioned :
0 replaced with No
1 replaced with Yes
All the above mentioned values of 0 and 1 are valid. No impossible values have been observed in the data column.
12. Education : This attribute gives information of the quali​cation(education) level of the employees. The data column had values
ranging from 1 to 4. These values are made more sensible by assigning a category which is meaningful in the real world. Below are the categories mentioned :
1 replaced with High School
2 replaced with Graduate
3 replaced with Post-Graduate
4 replaced with Master and Doctor
All the above mentioned values ranging from 1 to 4 are valid education levels. No impossible values have been observed in the data column.
13. Son : This attribute gives information of the number of children the employee has. The data column had values ranging from 0 to 4. No impossible values have been observed in the data column.
14. Social drinker : This attribute gives information whether the employee is a social drinker or no. The data column had values of 0 and 1. These values are made more sensible by assigning a category which is meaningful in the real world. Below are the categories mentioned :
0 replaced with No
1 replaced with Yes
All the above mentioned values of 0 and 1 are valid. No impossible values have been observed in the data column.
15. Social smoker : This attribute gives information whether the employee is a social smoker or no. The data column had values
of 0 and 1. These values are made more sensible by assigning a category which is meaningful in the real world. Below are the categories mentioned :
0 replaced with No
1 replaced with Yes
All the above mentioned values of 0 and 1 are valid. No impossible values have been observed in the data column.
16. Pet : This attribute gives information of the number of pets the employee has. The data column had values ranging from 0 to
8. No impossible values have been observed in the data column.
17. Weight : This attribute gives information of the weight of the employee in kilograms. The data column had values ranging
from 56 kilograms to 108 kilograms. No impossible values have been observed in the data column.
18. Height : This attribute gives information of the height of the employee in centime- tres. The data column had values ranging
from 163 centimeters to 196 centimeters. No impossible values have been observed in the data column.
19. Body mass index : This attribute gives information of the body mass index(BMI) of the employee. The data column had
values ranging from 19 to 38. No impossible values have been observed in the data column.
20. Absenteeism time in hours : This is the targeted output column of the project. This attribute gives information of the number
of hours an employee was absent on a particular day. The data column had values ranging from 0 to 120. A work day consists of only 8 hours so values ranging from 0 to 8 are considered as valid. Impossible values of greater than 8 were observed, which does not co-relate to any working day in the real world. The dataset contained 63 observations with this value, and all have been removed to make the dataset more meaningful.
