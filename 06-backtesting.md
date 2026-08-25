# 백테스팅 및 성과 분석

## 오늘 배운 것

- 백테스팅이란 과거 데이터로 전략을 미리 검증해보는 과정이라는 개념
- 누적수익률(cumulative return)과 최대낙폭(MDD, Max Drawdown) 계산법
  ```python
  cum_return = (1 + df["return"]).cumprod()
  mdd = (cum_return / cum_return.cummax() - 1).min()
  ```
- 미래 데이터를 참조하는 실수(look-ahead bias)를 피해야 하는 이유
- 백테스팅 결과를 그래프로 시각화해서 전략의 안정성을 확인하는 법

## 느낀 점

수익률만 좋다고 좋은 전략이 아니라, 손실 구간(MDD)이 얼마나 깊고 길었는지가 실전에서는 더 중요하다는 걸 알게 됐다. 앞으로 전략을 짤 때 수익률과 리스크를 같이 봐야겠다.
