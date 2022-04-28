
# Project 1: Analyse statewide participation and recommend where money is best spent to improve SAT participation Rate.

Problem Statement:
- Analysing trend in SAT and ACT participation Rate statewide and what are the areas of opportunity to increase participation rate.

Background
The SAT and ACT are standardised test that are accepted by universities and college in United States for admission. The test are used to assess a student readiness and ability for university. The SAT went through a massive revision and redesign in 2016 to align its format towards ACT.
The SAT focuses on 2 main topics, Evidence based reading and writing and Maths.
([*source*](https://sat.ivyglobal.com/new-vs-old/)).

While the ACT focuses on English, Math, Reading and Science.
[(*source*)](https://www.manhattanreview.com/act-format/#:~:text=The%20five%20sections%20of%20the,and%2035%20minutes%20to%20finish.)


Due to recent covid pandemic that led to many high school closed and remotely teaching, a growing number of college and universities are temporary waiving standardised test requirements.
There have also been criticism from education reform groups that felt that wealthier students were able to do better due to the ability to afford quality and expensive prep exam and coaching.
[(*source*)](https://www.nytimes.com/article/sat-act-test-optional-colleges-coronavirus.html?msclkid=880e684fc6ff11ecbb410e1c315d2d26)
This would slowly result in an increase to shift away from such test requirement for fairer playing ground.
There were also repeated cheating scandals,  bribery scandals and hiring of impostors to take the exam which ultimately question the integrity and reliability of the test.
[(*source*)](https://www.washingtonpost.com/education/2019/03/19/is-it-finally-time-get-rid-sat-act-college-admissions-tests/)

Dataset Selected:
- sat_2017.csv
- sat_2018.csv
- sat_2019.csv
- act_2017.csv
- act_2018.csv
- act_2019.csv

The dataset provides the total state participation rates as well as the average total score students at a national level.
This data will be used to determine the relationship and find what are the opportunities for SAT to increase its participation rate.

Data Dictionary

|Feature|Type|Dataset|Description|
|---|---|---|---|
|**state**|string|act_sat_total|All the state located in United States of America.
|**act_2017_participation**|float|act_2017 dataset|Total percentage of ACT participation of the respective states in 2017. (Units percent in two decimal place 1.00 means 100%. Participation of 100% indicates that ACT is mandatory in the respective state)
|**act_2017_composite**|float|act_2017 dataset|Annual average ACT scores of the students that participated in their respective state. ACT composite score range between 1 to 36 (1 being the lowest and 36 being perfect score)
|**act_2018_participation**|float|act_2018 dataset|Total percentage of ACT participation of the respective states in 2018. (Units percent in two decimal place 1.00 means 100%. Participation of 100% indicates that ACT is mandatory in the respective state)
|**act_2018_composite**|float|act_2018 dataset|Annual average ACT scores of the students that participated in their respective state.ACT composite score range between 1 to 36 (1 being the lowest and 36 being perfect score)
|**act_2019_participation**|float|act_2019 dataset|Total percentage of ACT participation of the respective states in 2019. (Units percent in two decimal place 1.00 means 100%. Participation of 100% indicates that ACT is mandatory in the respective state)
|**act_2019_composite**|float|act_2019 dataset|Annual average ACT scores of the students that participated in their respective state.ACT composite score range between 1 to 36 (1 being the lowest and 36 being perfect score)
|**sat_2017_participation**|float|sat_2017 dataset|Total percentage of SAT participation of the respective states in 2017. (Units percent in two decimal place 1.00 means 100%. Participation of 100% indicates that SAT is mandatory in the respective state)
|**sat_2017_ebrw**|integer|sat_2017 dataset|Annual average evidence based reading and writing(EBRW) score of all students who took SAT in 2017. EBRW score ranges between 200 to 800, with 200 being the lowest and 800 being the highest.
|**sat_2017_math**|integer|sat_2017 dataset|Annual average math score of all students who took SAT in 2017. Math score ranges between 200 to 800, with 200 being the lowest and 800 being the highest.
|**sat_2017_total**|integer|sat_2017 dataset|The sum of total annual average EBRW and math score obtained by students in their respective states. The sum of both subjects ranged between 400 to 1600 where total score of 400 is the lowest and 1600 is the highest.
|**sat_2018_participation**|float|sat_2018 dataset|Total percentage of SAT participation of the respective states in 2018. (Units percent in two decimal place 1.00 means 100%. Participation of 100% indicates that SAT is mandatory in the respective state)
|**sat_2018_ebrw**|integer|sat_2018 dataset|Annual average evidence based reading and writing(EBRW) score of all students who took SAT in 2018. EBRW score ranges between 200 to 800, with 200 being the lowest and 800 being the highest.
|**sat_2018_math**|integer|sat_2018 dataset|Annual average math score of all students who took SAT in 2018. Math score ranges between 200 to 800, with 200 being the lowest and 800 being the highest.
|**sat_2018_total**|integer|sat_2018 dataset|The sum of total annual average EBRW and math score obtained by students in their respective states. The sum of both subjects ranged between 400 to 1600 where total score of 400 is the lowest and 1600 is the highest.
|**sat_2019_participation**|float|sat_2019 dataset|Total percentage of SAT participation of the respective states in 2019. (Units percent in two decimal place 1.00 means 100%. Participation of 100% indicates that SAT is mandatory in the respective state)
|**sat_2019_ebrw**|integer|sat_2019 dataset|Annual average evidence based reading and writing(EBRW) score of all students who took SAT in 2019. EBRW score ranges between 200 to 800, with 200 being the lowest and 800 being the highest.
|**sat_2019_math**|integer|sat_2019 dataset|Annual average math score of all students who took SAT in 2019. Math score ranges between 200 to 800, with 200 being the lowest and 800 being the highest.
|**sat_2019_total**|integer|sat_2019 dataset|The sum of total annual average EBRW and math score obtained by students in their respective states. The sum of both subjects ranged between 400 to 1600 where total score of 400 is the lowest and 1600 is the highest.

Findings
- There were a total of 5 states namely, New Mexico, Alabama, Tennessee, Arkansas, Oklahome that experience consecutive growth of 10% or more in SAT participation rate within the 3 year period. While ACT participation only had 1 state, Arizona that grew more than 5% year on year.
- The total amount of states that have participation rate of more than 80% have been growing rapidly over the 3 year period. While ACT on the other hand, is facing a slight decline for states with more than 80% participation rate.
- West Virginia shifted from 28% participation rate in 2018 to 99% participation in 2019. Based on the admission data by West Virginia University, the admitted students fall within the top 35% nationally on SAT while students who got admitted throught ACT fall within the top 42%. [(*source*)](https://www.thoughtco.com/west-virginia-university-admissions-788220)

- SAT have 1 state, Nevada that have been experiencing consecutive fall in state participation rate at a rate of 11%-13% year on year.
- There is a strong negative correlation between ACT and SAT participation rate for all 3 years.
- There is a strong negative correlation between ACT and its composite scores for all 3 years.
- There is a strong negative correlation between SAT and its total scores for all 3 years.
- This could be due to students who volunteered to participate in the low state participation rate are well prepared. While mandatory states forces students who are motivated as well as unmotivated to participate in the testing.

Conclusion/Recommendation
- Overall, the participation rate for the SAT have been increasing strongly over the past 3 years. Based on the findings, more states are choosing SAT over ACT as derived from the number of state with more than 80% participation rate increase as well as consistent growth rate.
- There is a strong negative relationship between ACT and SAT participation rate which indicates a fall in ACT might result in a rise in SAT.
- There is also a strong negative relationship between SAT/ACT participation rate and total score. This could be due to well-prepared and motivated students choosing to volunteer and participate in the non-mandatory states.

Recommendation
In an aim to improve the SAT participation rate, the college board may consider the following:

- Provide more resources such as classes at subsidised rate by leveraging on online platform to boost student results.
- Provide mock test to allow students to gauge how they are doing, especially in mandatory states.
- Enforce stricter checks for imposters and heavy penalty for offenders to ensure the integrity and reliability of the test participants and results.
- Focus more resources and support in California in hope to increase its participation rate. This is because California state has the most number of prestige universities. Ontop of that, California state participation have been increasing consistently year on year with participation rate above 50% for the past 3 years. The falling participation rate of ACT in California further reinforce choosing California as the ideal state.  
## Authors

- [@zacharykwek15](https://github.com/zacharykwek15)
