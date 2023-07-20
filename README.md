# Probono-AI
사회적 약자를 위한 생활예보서비스 제공 부문 중, 날씨 및 행사 정보를 결합한 관심 지역 인구밀집도 예측 모델

# 수행과정

## 목표 설정: 서울특별시 동 단위 행정구역 인구밀집정보를 예측.

> 필요 데이터셋 : 과거 인구 밀집 정보, 과거 날씨 정보, 초단기 미래 날씨 정보, 초단기 미래 행사 정보 등의 csv 파일을 사용한다.

## 데이터 셋 전처리

> Column 파악 : 어떤 데이터가 의미 있는 데이터인지 파악한다.
> 의미 있는 데이터로 분류 후 새로운 데이터프레임 생성한다.
> 결측치 파악 및 결측치 채운다.

## 결측치 제거 한 뒤 시각화

> 특정 데이터의 경우, 극소수의 결측을 보일 뿐더러, 기존의 추정치가 없다면 기계학습을 통한 예측이 어려우므로 삭제한다.

## 샘플 데이터를 통한 전이학습

> 해당 모델의 경우 RNN 방식을 사용한다, 따라서 LSTM, GRU 2가지를 사용해보고, 정확도가 높은 모델을 선정하여, 전이학습 과정을 가지도록 한다.

## 모델 훈련 및 모델 분석
> 모델 훈련 : 훈련 데이터와 검증 데이터를 사용하여 모델의 파라미터를 조정하고 최적화하는 과정을 거친다.

> 모델 분석 : 테스트 데이터를 사용하여 모델의 성능을 평가하고 결과를 분석한다.