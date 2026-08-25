# 머신러닝 기초

## 오늘 배운 것

- 지도학습(supervised learning)과 비지도학습의 차이
- 학습 데이터를 train/test로 나누는 이유와 `train_test_split` 사용법
- 회귀(regression)와 분류(classification)의 차이 — 주가 "값"을 예측할지, 상승/하락 "방향"을 예측할지
- 과적합(overfitting)이 생기는 이유와 이를 막기 위한 교차검증(cross-validation) 개념

## 느낀 점

퀀츠에 머신러닝을 적용할 때는 모델 성능보다 "데이터 누수(data leakage)"를 조심해야 한다는 이야기가 인상 깊었다. 미래 정보가 학습 데이터에 섞이면 실전에서는 전혀 안 통하는 모델이 될 수 있다는 걸 명심해야겠다.
