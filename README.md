# 202045801 강병준 인공지능응용 기말과제

## 네이버 영화 리뷰 데이터셋 분류 모델
### 레퍼런스
https://wikidocs.net/44249
https://www.kaggle.com/competitions/2024-ml-project-korean/overview

### 데이터셋
네이버 영화 리뷰 데이터셋(NSMC: Naver Sentiment Movie Corpus)
긍정(1)과 부정(0) 레이블이 균등하게 분포

### 데이터셋 전처리
1. 자연어 전처리
  1.1. 정규표현식으로 불필요한 문자 제거
  1.2. OKT를 이용한 Tokenization
  1.3. 불용어 제거
2. 단어 임베딩
3. 문장 벡터화
4. 차원 축소
   
### 분류 모델 학습
1. 로지스틱 회귀
2. SVM
3. 다층 퍼셉트론
   
### 모델 선정: SVM
SVM, SVM + TF-IDF, 균형옵션 추가 등을 통한 최적화 작업
LinearSVM으로 메소드 변경 및 GridSearchCV를 통한 하이퍼파라미터 최적화
최적화된 SVM (GridSearchCV)	82.76%	Precision: 0.83, Recall: 0.82, F1-Score: 0.83
