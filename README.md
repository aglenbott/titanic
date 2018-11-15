# Titanic

| Variable    | Definition                          | Type        | Key                                            | Notes                                                                                                                                                                                           |
|-------------|-------------------------------------|-------------|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| PassengerId |                                     | discrete    |                                                |                                                                                                                                                                                                 |
| Survived    | Survival                            | discrete    | 0 = No, 1 = Yes                                |                                                                                                                                                                                                 |
| Pclass      | Ticket class                        | categorical | 1 = 1st, 2 = 2nd, 3 = 3rd                      | A proxy for socio-economic status (SES)                                                                                                                                                         |
| Name        | Name                                | discrete    |                                                |                                                                                                                                                                                                 |
| Sex         | Sex                                 | categorical |                                                |                                                                                                                                                                                                 |
| Age         | Age                                 | discrete    |                                                | Age is fractional if less than 1. If the age is estimated, is it in the form of xx.5                                                                                                            |
| SibSp       | Number of siblings/spouses on board | discrete    |                                                | The dataset defines family relations in this way... Sibling = brother, sister, stepbrother, stepsister Spouse = husband, wife (mistresses and fiancés were ignored)                             |
| Parch       | Number of parents/children on board | discrete    |                                                | The dataset defines family relations in this way... Parent = mother, father Child = daughter, son, stepdaughter, stepson Some children travelled only with a nanny, therefore parch=0 for them. |
| Ticket      | Ticker number                       | discrete    |                                                |                                                                                                                                                                                                 |
| Fare        | Passenger fare                      | continuous  |                                                |                                                                                                                                                                                                 |
| Cabin       | Cabin number                        | discrete    |                                                |                                                                                                                                                                                                 |
| Embarked    | Port of embarkation                 | categorical | C = Cherbourg, Q = Queenstown, S = Southampton |                                                                                                                                                                                                 |
|             |                                     |             |                                                |                                                                                                                                                                                                 |
|             |                                     |             |                                                |                                                                                                                                                                                                 |

## Statistical question
Does a passenger's `Sex` have an impact on their chance of `Survival`?

## Hypotheses

H<sub>0</sub>: Any difference between male passenger survival rate and
 female passenger survival rate is caused by chance.

H<sub>1</sub>: Any difference between male passenger survival rate and
 female passenger survival rate is not caused by chance, but is 
actually statistically significant.

## Better hypothesis formulation

H<sub>0</sub>:  The variables `Sex` and `Survival` are independent.
They have no relationship, and the observed difference between the proportion 
of males and females who survived the sinking of the Titanic (55.31%) 
was due to chance.

H<sub>1</sub>: The variables `Sex` and `Survival` are not independent.
The difference in survival rates of 55.31% was not due to chance,
and sex does help predict survival.