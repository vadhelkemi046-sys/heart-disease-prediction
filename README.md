# Heart Disease Prediction using Machine Learning

Predicts whether a patient has heart disease from 13 clinical features using K-Nearest Neighbors and Random Forest.

Based on my research paper "Heart Disease Prediction Using Machine Learning" (2nd Best Paper Presentation Award, International Conference of Emerging Vista's of Computer Science, IT and Management in 21st Century, Parul University, March 2024).

## Dataset
Heart disease dataset, 303 patients, 13 features, target = heart disease (yes/no). Included as Heart.csv.

## Method
- Cleaning: dropped the index column, filled 6 missing values with the most common value, encoded categorical columns, standardised numeric columns
- 80/20 train/test split
- Models: K-Nearest Neighbors (K=12) and Random Forest (10 trees)

## Results
| Model | Result in the paper | This notebook (random_state=0) |
|---|---|---|
| KNN (K=12) | 86.89% | 77.05% |
| Random Forest (10 trees) | 81.97% | 80.33% |

Numbers differ because the paper used a different version of the dataset and split. The test set has only 61 patients, so results change noticeably with the split.

## Run
pip install pandas scikit-learn seaborn matplotlib notebook
jupyter notebook# heart-disease-prediction
