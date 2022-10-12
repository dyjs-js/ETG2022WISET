# 앗! 조심해-딥러닝 기반의 객체 탐지를 통한 보행자 안전사고 예방

## **개발 배경**

- 보행 중 스마트폰 사용률이 높은 가운데 안전사고의 위험성도 높음
- 인도 내 안전사고에 대해서는 적극적인 예방책이 부족함
- 추가적인 설비없이 스마트폰을 활용하여 안전사고를 줄일 수 있는 방법에 대해 고민

## **시연영상**

- (https://youtu.be/NlyxRDEqX3Y)

## **개발환경**

![개발환경및언어](https://user-images.githubusercontent.com/85267081/189961950-35e553bc-c90b-4c72-b856-a9a2aed1bbb5.jpg)

## **System Architecture**

딥러닝 객체 탐지 모델인 YOLOv5를 활용하여 이미지/영상에서 Bollard, 전동킥보드를 탐지하고 안드로이드 앱을 통해 스마트폰 사용자에게 알림

(YOLOv5 : YOLO의 이전 버전 대비 우수한 성능과 빠른 실행 속도)

![시스템구성및아키텍쳐](https://user-images.githubusercontent.com/85267081/188958851-d922d60f-6792-43de-9026-c0ab6b20f036.jpg)

## **주요기능**

- 실시간으로 인도 내 장애물(Bollard, 전동킥보드)을 탐지하여 안드로이드 앱을 통해 스마트폰 사용자에게 알림(음성, 진동)으로써 인도 내 스마트폰 사용 보행자들의 안전사고의 발생률을 낮춤
![주요기능과정이미지](https://user-images.githubusercontent.com/85267081/190176511-a1a3ae70-e9ba-4e1e-8c65-1a9bb56cb4f7.jpg)

[(앗!조심해 Android app Github)](https://github.com/Kimsunjeung/android_YOLOv5_app.git)   

[(YOLOv5 학습 모델 탑재 App Download)](https://drive.google.com/file/d/1bb6ZgBVjNafqedZKAWg1dZhfvjU0866M/view?usp=sharing)
- 해당 apk 파일을 다운로드 후 안드로이드 스마트폰에 직접 설치하여 실행 가능

## **Dataset**

### **Bollard**

#### 이미지 및 좌표 정보 > AI-Hub 사이트(https://aihub.or.kr) '인도 보행 영상' Dataset에서 추출

### **전동킥보드**

#### 이미지 > Image crawling을 통해 구글, 네이버에서 공유킥보드 이미지 630장 + 직접 핸드폰으로 촬영한 이미지 33장

#### 좌표정보 > roboflow.com에서 1299장 직접 annotation함(Dataset명 : bolles)

![image](https://user-images.githubusercontent.com/85267081/188961381-b5537d43-61c6-4208-80d9-924376e0d5e6.png)

## **향후 과제**
최근 공개된 YOLOv7 알고리즘을 적용하여 현 모델과 탐지 성능을 비교 및 성능 개선

![sun-9-v7_resized](https://user-images.githubusercontent.com/85267081/190104766-7010c650-0408-4d3c-944c-ca9b52a7766a.gif)
YOLOv7 학습모델 적용 결과 

## **ETG(EoltTeuGi)팀소개**

| 구 분 | 이 름    | 이 메 일              | 메 인 역 할                     | 공 통 역 할                 |
| ----- | -------- | --------------------- |-------------------------------- |-----------------------------|
| 팀 장 | 김 선 정 | <toursun@naver.com>   |Dataset 생성, Android app 개발    | DNN Transfer Learning|
| 팀 원 | 주 은 정 | <hahory0@naver.com>   |데이터 전처리                     |     
| 팀 원 | 연 지 수 | <dydy11642@gmail.com> |시연 영상 제작                    |    
| 팀 원 | 이 서 영 | <zjarhk21@naver.com>  |Android app troubleshooting      |    
