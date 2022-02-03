# Body-Morphometry-Kidney-and-Tumor
[**MOAI 2021 Body Morphometry AI Segmentation Online Challenge**](https://www.kaggle.com/c/body-morphometry-kidney-and-tumor/data)

#### 'Remember' Team : 이승리, 서원진, 최재홍

----

## 기간

21.09.11-21.09.6
<br><br>

## 당시 배경 지식 

단순 분류/회귀 구현 정도 (정말 기초지식만 보유)
<br><br>

## 목표

많이 공부하고, 적어도 중간은 가보자
<br><br>

## 결과 

Rank : 10/27
<br><br>

## 과정

1) Dicom format에 대해 공부

2) Segmentation에 대해 공부

3) Data Preprocessing 코드 구현

4) Model train 및 test 코드 구현

5) 조사 및 여러 실험을 해보며 잘 되는 WW(Window Width:픽셀값의 범위)와 WL(Window Center:기준이 되는 픽셀값)을 찾기

6) Augmentation 실험적 적용을 통해 효과있는 Augmentation만 남기기

7) 여러 Model 실험

8) 배포 전 데이터가 3D였다는 점을 참고해 3D Model 적용
<br>

## 알게된 점

- Dicom format은 다양한 정보가 담겨있는 format으로 쓰고자 하는 정보만 뽑아 쓸 수 있다는 것

- Segmentation model의 output channel은 class수와 같다는 것(처음에 이걸 몰라 많이 헤맸다)

- Data에 따라 Augmentation이 악영향을 미칠수도 있다는 것

- U-net, Dice loss

- Data post-processing도 필요하단 것

- 의료데이터는 Case별로 Dataset을 나눠야한다는 것

- 데이터 편향문제의 
<br>

## 아쉬운 점

- 3D모델 적용을 통해 눈에 띄는 성능향상을 보였지만 다시 2D로 나눠 제출 format에 맞추는 것을 실패

- 3D모델을 가져다 인풋,아웃풋에 대한 layer만 수정했을뿐 별다른 customizing을 못 한 것

- 수상팀 코드공개를 안 해 다른 팀들이 어떻게 접근했는 지 알 수 없었던 것
<br>

## 향후계획

- 데이터 편향문제 해결방안을 찾아볼 것

- 3D Model로 제출양식 맞춰서 제출해볼 것
