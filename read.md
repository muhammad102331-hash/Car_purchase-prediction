# Car Purchase Analysis Insights (Simple Language)

## What this analysis is about
This project studies customer data to understand who is more likely to buy a car.

## Data overview
- Total customers: 1000
- Columns used: Gender, Age, AnnualSalary, Purchased
- Data quality: no missing values and no duplicate rows

This means the dataset is clean and trustworthy for decision-making.

## Key facts from results
- Purchase rate is about 40.2%.
	Around 4 out of 10 customers bought a car.
- Gender is balanced.
	Female: 516, Male: 484.
- Average customer age is about 40 years.
- Average annual salary is about 72,689.

## Insights from charts

### 1) Salary distribution by gender
The salary spread looks similar for males and females, with both groups covering low to high salary ranges.

### 2) Age distribution by gender
Both genders appear across most age groups, so age coverage is broad and not limited to one group.

### 3) Salary vs purchase (hist chart)
People with higher salary bands appear more likely to purchase than those in lower salary bands.

### 4) Age vs purchase (hist chart)
Purchase likelihood increases with age. Older customers are more likely to buy compared to younger customers.

### 5) Correlation check with purchase
- Age correlation with purchase: 0.616
- Salary correlation with purchase: 0.365

Simple meaning: age has a stronger connection with buying behavior than salary.

## Model performance results

### Logistic Regression
- Accuracy: 83.67%
- Correct predictions: 251 out of 300

### KNN (k = 12, elbow choice)
- Accuracy: 91.67%
- Correct predictions: 275 out of 300

### KNN (GridSearch best k = 7)
- Accuracy: 91.33%
- Correct predictions: 274 out of 300

### SVM (GridSearch best: C = 1, kernel = rbf)
- Accuracy: 91.67%
- Correct predictions: 275 out of 300

## Final takeaway for non-technical readers
- The strongest buying signal is age.
- Salary also influences buying, but less than age.
- The prediction system works well (about 92% accuracy with best models).
- For marketing and sales targeting, prioritize older customers and also consider higher-income segments.

## Note
Model scores can change slightly if the train/test split changes, but the overall trend remains similar.
