# kaggle-titanic
This project is a part of my personal Data Science portifolio and uses the Titanic dataset provided by [Kaggle](https://www.kaggle.com/).

#### -- Project Status: [Active]

## Project Intro/Objective
The purpose of this project is to create a model which can predict whether a given titanic passenger survived the sinking based solely on basic information that were present in the trip files.

### Methods Used
* Inferential Statistics
* Machine Learning
* Data Visualization
* Feature Engineering
* Ensemble Modeling

### Technologies
* Python
* Jupyter Notebook
* Scikit-Learn
* Pandas
* Numpy
* XGBoost

## Project Description
(Provide more detailed overview of the project.  Talk a bit about your data sources and what questions and hypothesis you are exploring. What specific data analysis/visualization and modelling work are you using to solve the problem? What blockers and challenges are you facing?  Feel free to number or bullet point things here)

## Dataset
### Raw Data Dictionary (provided by [Kaggle](https://www.kaggle.com/))
| Cariable | Definition                                 | Key                                            |
|----------|--------------------------------------------|------------------------------------------------|
| survival | Survival                                   | 0 = No, 1 = Yes                                |
| pclass   | Ticket class                               | 1 = 1st, 2 = 2nd, 3 = 3rd                      |
| sex      | Sex                                        |                                                |
| Age      | Age in years                               |                                                |
| sibsp    | # of siblings / spouses aboard the Titanic |                                                |
| parch    | # of parents / children aboard the Titanic |                                                |
| ticket   | Ticket number                              |                                                |
| fare     | Passenger fare                             |                                                |
| cabin    | Cabin number                               |                                                |
| embarked | Port of Embarkation                        | C = Cherbourg, Q = Queenstown, S = Southampton |

### Data Dictionary after feature engineering
| Feature                                                                                                                                                                                                                                                                                                    | Definition                                                        | Key                       |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------|---------------------------|
| Mates_Performance                                                                                                                                                                                                                                                                                          | Survival performance of known travel mates                        |                           |
| Pclass                                                                                                                                                                                                                                                                                                     | Ticket class                                                      | 1 = 1st, 2 = 2nd, 3 = 3rd |
| Pclass_1, Pclass_2, Pclass_3,                                                                                                                                                                                                                                                                              | Dummies for passenger class                                       |                           |
| Age                                                                                                                                                                                                                                                                                                        | Age in years                                                      |                           |
| Age Group_Adult, Age Group_Child, Age Group_Elderly, Age Group_Senior, Age Group_Teenager, Age Group_Young_Adult                                                                                                                                                                                           | Dummies for Age Group                                             |                           |
| SibSp                                                                                                                                                                                                                                                                                                      | # of siblings or spouses aboard the Titanic                       |                           |
| Parch                                                                                                                                                                                                                                                                                                      | # of parents or children aboard the Titanic                       |                           |
| Fare                                                                                                                                                                                                                                                                                                       | The total passenger fare                                          |                           |
| numFamilyMembers                                                                                                                                                                                                                                                                                           | Total size of a passenger family aboard                           |                           |
| HasFamily                                                                                                                                                                                                                                                                                                  | Dummy that tells whether a passenger has any family member aboard | 1 = Yes, 0 = No           |
| AverageFare                                                                                                                                                                                                                                                                                                | The total fare divided by the total family size                   |                           |
| Age*Class                                                                                                                                                                                                                                                                                                  | The age times the passenger class                                 |                           |
| Sex_female, Sex_male,                                                                                                                                                                                                                                                                                      | Dummies for gender                                                |                           |
| CabinType_A, CabinType_B, CabinType_C, CabinType_D, CabinType_E, CabinType_F, CabinType_G, CabinType_T, CabinType_Unknown                                                                                                                                                                                  | Dummies for Cabin Type                                            |                           |
| Grouped_Title_Master, Grouped_Title_Miss, Grouped_Title_Mr, Grouped_Title_Mrs, Grouped_Title_Rare                                                                                                                                                                                                          | Dummies for Grouped Name Titles                                   |                           |
| Name Title_Mr, Name Title_Mrs, Name Title_Master, Name Title_Miss, Name Title_Capt, Name Title_Col, Name Title_Don, Name Title_Dona, Name Title_Dr, Name Title_Jonkheer, Name Title_Major, Name Title_Mlle, Name Title_Mme, Name Title_Lady, Name Title_Ms, Name Title_Rev, Name Title_Sir, Name Title_the | Dummies for Name Titles                                           |                           |
| Embarked_C, Embarked_Q, Embarked_S,                                                                                                                                                                                                                                                                        | Dummies for port of embark                                        |                           |
| Survived                                                                                                                                                                                                                                                                                                   | Survival                                                          | 1 = Yes, 0 = No           |## Needs of this project

## Needs of this project
- frontend developers
- data exploration/descriptive statistics
- data processing/cleaning
- statistical modeling
- writeup/reporting

## Getting Started
1. Clone this repo (for help see this [tutorial](https://help.github.com/articles/cloning-a-repository/)).
2. Raw Data is being kept in [datasets](https://github.com/ronyefreitas/kaggle-titanic/tree/master/datasets) within this repo.
3. Follow setup [instructions](Link to file)


## Contact
ronye.freitas@gmail.com
