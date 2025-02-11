﻿# 사조참치

**Portfolio Visualizer Localization (가제)**

포트폴리오 배분, 리스크, 수익률 분석에 편리한 웹사이트 ‘Portfolio Visualizer’의 백테스팅 기능을 한국 자산에 맞게 수정

## 팀원

1. 김민제 (리스크)
2. 권민회 (리스크)
3. 손유민 (리스크)
4. 박한규 (IT)
5. 백종성 (IT)

## 배경 및 문제 정의

- 현상 / 상황
  - 대부분의 자산 가격이 상승하던 2021년과 달리 불황이 닥치면서 전반적인 자산 가격이 떨어짐에 따라 더 면밀한 포트폴리오 분석이 요구됨.
- 핵심 문제 및 원인
  - 사회 초년생 등 투자 경험이 상대적으로 부족한 개인 투자자들이 단축된 시간 내에 원하는 포트폴리오를 분석하기 어려움.
  - 해외 주식들의 경우, Portfolio Visualizer 등 사이트를 활용해 무료로 정적, 동적 자산 배분 전략들을 백테스트를 빠른 속도로 시행할 수 있음. 그러나 국내 종목들의 경우, 자산 배분 백테스트를 무료로 빠르게 시행할 수 있는 사이트가 없음.

## 기대효과

- As-is
  - 고객에게 자산 배분 현황에 대해 설명할 때, 포트폴리오의 시각화 범위가 한정됨.
  - 기존 국내 수익률 계산 서비스는 한 가지 자산에 한정되거나, 위험 지표까지 안내해주지 않는 경우가 대다수임.
- To-be
  - 여러 포트폴리오를 한 화면에서 분석하여 추천 포트폴리오의 수익을 설명하기 용이하고, 시각화를 통해 고객의 불안감을 해소시킬 수 있음.
  - 여러 자산을 포함한 포트폴리오의 분석이 가능해지고, 위험 지표까지 비교할 수 있게 하여 좀 더 다채로운 포트폴리오 구성이 가능해짐.

## 분석모델

- 활용데이터 (Input)
  1.  주가 데이터: KRX(pykrx), Naver Finance, FinanceDataReader
  2.  금, 은, WTI 데이터: Naver Finance, Yahoo Finance, Investing.com등
- 적용하는 AI 기능

  1.  강화학습(Reinforcement Learning)을 활용한 주가예측

- 예상 적용 결과
  1.  과거 데이터 이용(백테스팅): 자산 동향 쉽게 파악 가능
      - 자산 배분 백테스트에 최적화된 백테스팅 툴 개발 가능함.
  2.  유명 투자 전략들의 백테스팅 성과와 비교 분석 가능
      - 영구 포트폴리오, 올웨더 같은 **정적 자산 배분 전략**을 만들 수 있음.
      - 듀얼 모멘텀과 같은 **동적 자산 배분 전략** (마켓 타이밍 전략)들 관련 빠르게 백테스트 결과물 도출 가능함.
      - **즉 데이터 업로드하여 백테스트 가능**
  3.  관심 투자 자산의 변동성, VaR, 수익률, MDD 등의 정보를 편리하게 확인 가능
