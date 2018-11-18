
Localization ; 
=============
>내(Robot, itself) 위치를 추정하기위한 방법론  

## 1. Kalman filter
* Rudolf E.Kalman has developed the Kalman filter.
  - Noise 가 포함된 선형 시스템(Linear System)에서 대상체의 상태를 추적하는 재귀 필터(Recursive filter)를 말함.
    + Bayes Theorem 기반, 모델을 상정하고 이 모델을 이용하여 이전 상태로부터 현재 시점의 상태를 Prediction.  
           - Bayse Theorem :  
               P(A|B) = P(B|A)P(A)/P(B)
    + 그 다음 앞 단계의 예측값과 외부 계측기로 얻은 실제 측정값 사이의 오차(error)를 이용해 더 정확한 상태의 상태값을 추정하는 보정(update) 단계를 거친다.
    + Recursive 하게 반복해서 정확도를 높여감.
  - 단, 칼만필터는 선형 시스템(Linear System)에만 적용가능.  
  보통 로봇과 센서는 대부분 비선형 시스템(Non-linear System).  
  -- 이를 해결하기 위해  **EKF(Extended Kalman filter_확장칼만필터)** 를 많이 사용함.  
  -- EKF의 정확성을 보완한 UKF(Unscented Kalman filter_무향 칼만필터), 속도를 개선한 Fast Kalman filter 등 다수.  
  -- Particle filter와 함께 사용하는 RBPF(Rao-Blackwellized Particle Filter) 등 다른 알고리즘과 함께 사용됨.

## 2. Particle filter

* 1
    - 2
    	+ 3
