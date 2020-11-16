# DOG_FINDER (유기견 입양 프로젝트)
**: image classification for dogs

CSLEE에서 언어 시각 AI 전문가 양성과정에서 미니프로젝트로 '유기견 입양 프로젝트'를 진행하였습니다.

유기견을 입양할 때, 개의 품종이 중요하다는 분석결과를 얻어냈습니다.

그런데 유기견은 품종이 제대로 표시되지 않은 경우가 많아서, 이미지로 개의 품종을 분류하는 모델을 만들기로 했습니다.

Keras API를 사용하여, 딥러닝 모델로 개의 이미지를 품종별로 구별하였습니다.

학습환경은 Kaggle notebook에서 진행하였습니다. (GPU on)

# 모델
Inception V3, xception 이라는 두개의 학습된 모델을 가져와서, 전이학습함.
<img width="1061" alt="스크린샷 2020-11-16 오후 8 28 24" src="https://user-images.githubusercontent.com/66561385/99247641-95bfd480-284a-11eb-8ef2-2fcf4d0c3819.png">

# 데이터
kaggle 데이터 12000여장, 유기견 데이터 14000장을 사용함.
예시 : kaggle images
<img width="1172" alt="스크린샷 2020-11-16 오후 8 24 46" src="https://user-images.githubusercontent.com/66561385/99247135-dcf99580-2849-11eb-9dbd-15d3cb3f3ec6.png">

# 결과
kaggle의 경우 120종 구분에 85%, 유기견의 경우 83%의 정확도를 보임.
<img width="660" alt="스크린샷 2020-11-16 오후 8 24 29" src="https://user-images.githubusercontent.com/66561385/99247144-dec35900-2849-11eb-8121-e8535b5d44aa.png">
