# 25physics
2025 물리학 수행평가 코드 파일

1. 오실로스코프
  최종 버전: 1.4

  #동기#
  함수 발생기가 위상차(delta)=0임에도 다른 위상차 출력.
  -> CNN 회귀 분석으로 위상차 예측하고자 함.
  <img width="975" height="371" alt="image" src="https://github.com/user-attachments/assets/5c12765c-43e5-4d28-85f3-bef733149197" />
  [Figure 1] CNN processing diagram
  
  #train 과정#
  임의의 delta 값과 그에 해당하는 이미지를 무작위로 생성하여 train sample, val sample 제작
  -> train 12000장, val 2000장으로 학습.
  epochs=21로 진행.

  #사용 방법#
  run all로 모든 셀 동작
  마지막 셀에서 각진동수 비, 실험 이미지 절대 경로, 실험에서 세팅한 delta 값을 입력
  -> 마지막 셀에서 실험 이미지의 입력받은 각진동수 비에 해당하는 예측 delta 값과 그 값에 해당하는 리사주 도형, 원래 나와야 하는 리사주 도형 이미지를 출력함. 

  #코드 확인 방법#
  <img width="2528" height="1082" alt="image" src="https://github.com/user-attachments/assets/0129f0ac-b85c-4860-97e7-28ba5e90f465" />
< 오실로스코프. ver 1.3 클릭
  <img width="2554" height="945" alt="image" src="https://github.com/user-attachments/assets/19d39b4c-09b1-4e86-bcad-2f9ba84d73f0" />
< view file 클릭

!중요!
코드의 전체적인 틀은 직접 작성했으나, 코드에서 발생하는 오류를 잡기 위해 ChatGPT의 도움을 받은 코드이다.
