# CP1_11

### 1. 문제인식
        2022년 6월 말 USD/KRW 환율(이하 환율)이 1,300원대로 상승했다는 언론 보도를 접함.
        환율이 우리 경제에 미치는 영향이 큰 것을 알기에 한달 뒤의 환율을 예측해보기로 결정.


### 2. 데이터셋
        한국은행 경제통계시스템. 기간별 환율을 손쉽게 구할 수 있으며 최종환율 보다 조금 낮게 표시되어 보수적 접근이 가능함.


### 3. 예측기법
        메타(페이스북)에서 만든 예측 시스템 Prophet을 사용.


### 4. 결과 정리
        2022년 7월 5일 기준으로 한달 뒤인 8월 4일의 환율이 1,320원을 돌파할 것으로 예상(8월 4일 매매기준율 환율: 1,308원)
        실제 8월 4일 매매기준율 환율은 1,308원. 그런데 그 보다 앞선 7월 15일에 1,320원을 돌파. 8월 18일에 다시 1,320원을 돌파.


### 5. 한계점
    - 예측개념: 예측 방법은 두 가지로 분류할 수 있는데 
               관측치를 기반으로 단 하나의 값을 나타내는 Deterministic Forecasting과 
               시계열의 확률분포를 추정 및 해당 분포에서 미래의 값을 추정하는 Probabilistic Forecasting이 있는데,
               이 중 Probabilistic Forecasting을 사용하지 않은 것이 아쉬움.
               본인은 Probabilistic Forecasting을 사용하고 싶었으나 코딩 능력이 부족하여 사용하지 못 함.
               
               
               A: Deterministic Forecasting                              B: Probabilistic Forecasting
<img src="https://user-images.githubusercontent.com/10494367/177470000-8afd3655-478b-43b3-aa12-c2b8d6711f40.jpg">


    - 예측기법: 구글에서 만든 신경망 모델을 사용하고 싶었으나 소스코드가 공개가 되어 있지 않아 사용하지 못 했음. 
                논문을 보고 구현할 수 있을 정도로 코딩실력을 높일 계획.
<img src="https://user-images.githubusercontent.com/10494367/177469987-ea9ee522-5e26-4848-9e93-839ffdbc1ec5.jpg">

