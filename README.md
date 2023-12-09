머신러닝 활용 현금흐름 중심 기업수명주기를 고려한 부실예측모형 연구
====================
(상장 중소기업과 비상장 외감중소기업 비교 중심)
-----------------------------

# 서론
## 기획배경
## 선행연구
## 차별점
## 부실정의
## 기업수명주기 (현금흐름관련) 정의
## 연구대상 중소기업 범위

# 본론 Workflow
## 1_데이터 수집 및 전처리
### 1_1. 부실판단
### 1_2. 기업수명주기판단
### 1_3. 파생변수
### 1_4. train_test_split
탐색적 데이터 분석(EDA; Exploratory Data Analysis)은 수시로 한다.
### 1_5. 결측치 처리
inf는 max로 대체, -inf는 min으로 대체
정규성 검사
정규성 -> fillna(mean 평균)
정규성X -> fillna(median 중앙값)
### 1_6. 이상치 처리 -> Winaorizing
기업수명주기별 부실별 Q-Qplot
일괄 양쪽 1%
### 1_7. Resampling; Undersampling; 쌍대표본방식 (∵ 데이터 불균형)
기업수명주기별 정상과 부실의 표본 수 일치
PCA? Oversmapling

## 2_Feature Selection
### 2_1. filter : t-test, correlation, VIF
### 2_2. scaling : minmax, standard
### 2_3. wrapper : forward, backward, stepwise
### 2_4. embedded : LASSO

## 3_Modeling
Logistic regression, Suport Vector Machine, RandomForest, Boosting, Bagging, LightGBM, XGboost, adaboost
## 4_Robustic 강건성평가

# 결론 Insight
