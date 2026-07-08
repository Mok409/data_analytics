# Titanic Data Analytics — Project Summary

## Dataset Overview

- Cleaned rows: **775**
- Columns: **16**

## Descriptive Statistics

|             |   count |   mean |    std |   min |   25% |   50% |   75% |   max |
|:------------|--------:|-------:|-------:|------:|------:|------:|------:|------:|
| passengerid |     775 | 445.81 | 260.12 |  1    | 213.5 |   450 | 670.5 |   891 |
| survived    |     775 |   0.34 |   0.47 |  0    |   0   |     0 |   1   |     1 |
| age         |     775 |  28.75 |  12.78 |  0.42 |  22   |    28 |  34   |    80 |
| sibsp       |     775 |   0.44 |   0.9  |  0    |   0   |     0 |   1   |     5 |
| parch       |     775 |   0.34 |   0.79 |  0    |   0   |     0 |   0   |     6 |
| fare        |     775 |  17.82 |  13.58 |  0    |   7.9 |    13 |  26   |    65 |
| has_cabin   |     775 |   0.15 |   0.35 |  0    |   0   |     0 |   0   |     1 |
| family_size |     775 |   1.78 |   1.42 |  1    |   1   |     1 |   2   |     8 |
| is_alone    |     775 |   0.65 |   0.48 |  0    |   0   |     1 |   1   |     1 |

## Survival by Class

|   pclass |   survival_rate |   passengers |
|---------:|----------------:|-------------:|
|        1 |        0.508929 |          112 |
|        2 |        0.486034 |          179 |
|        3 |        0.245868 |          484 |

## Survival by Sex

| sex    |   survival_rate |   passengers |
|:-------|----------------:|-------------:|
| female |        0.688525 |          244 |
| male   |        0.178908 |          531 |

## Business Insights

1. Dataset contains **775** passengers after cleaning.
2. Overall survival rate is **33.9%**.
3. Females survived at **68.9%**, males at **17.9%** — sex is the strongest predictor.
4. First-class survival **50.9%** vs third-class **24.6%** shows a strong class effect.
5. Passengers with a cabin record survived at **59.6%** — cabin data likely correlates with wealth.
6. Traveling alone: **27.0%** survival vs **46.7%** with family.
7. Embarkation port **'c'** had the highest survival rate.
8. Average passenger age: **28.7**; average fare: **$17.82**.
9. Fare–survival correlation: **0.23** (higher fare → higher survival).
10. Age–survival correlation: **-0.12** (weak; children slightly favored).
11. Recommendation: prioritize sex, class and fare as top features for any survival prediction model.
