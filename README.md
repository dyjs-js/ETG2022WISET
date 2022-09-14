# 딥러닝 기반의 객체 탐지 프로젝트 : 앗! 조심해

## **개발 배경**

- 보행 중 스마트폰 사용률이 높은 가운데 안전사고의 위험성도 높음
- 인도 내 안전사고에 대해서는 적극적인 예방책이 부족함
- 추가적인 설비없이 스마트폰을 활용하여 안전사고를 줄일 수 있는 방법에 대해 고민

## **시연영상**

- Youtube URL 추가하기

## **개발환경**

![개발환경및언어](https://user-images.githubusercontent.com/85267081/189961950-35e553bc-c90b-4c72-b856-a9a2aed1bbb5.jpg)

## **System Achitecture**

딥러닝 객체 탐지 알고리즘인 YOLOv5를 활용하여 이미지/영상에서 Bollard, 전동킥보드를 탐지하고 안드로이드 앱을 통해 스마트폰 사용자에게 알림

(YOLOv5 : YOLO의 이전 버전 대비 우수한 성능과 빠른 실행 속도)

![시스템구성및아키텍쳐](https://user-images.githubusercontent.com/85267081/188958851-d922d60f-6792-43de-9026-c0ab6b20f036.jpg)

## **주요기능**

- 실시간으로 인도 내 장애물(Bollard, 전동킥보드)을 탐지하여 안드로이드 앱을 통해 스마트폰 사용자에게 알림으로써 인도 내 스마트폰 사용 보행자들의 안전사고의 발생률을 낮춤

![주요기능과정이미지](https://user-images.githubusercontent.com/85267081/190093432-63d91fdf-c74b-42ed-ad15-7122534e265b.jpg)


## **Dataset**

### **Bollard**

#### 이미지 및 좌표 정보 > AI-Hub 사이트(https://aihub.or.kr) '인도 보행 영상' Dataset에서 추출

### **전동킥보드**

#### 이미지 > Image crawling을 통해 구글, 네이버에서 공유킥보드 이미지 630장 + 직접 핸드폰으로 촬영한 이미지 33장

#### 좌표정보 > roboflow.com에서 1299장 직접 annotation함(Dataset명 : bolles)

![image](https://user-images.githubusercontent.com/85267081/188961381-b5537d43-61c6-4208-80d9-924376e0d5e6.png)

## **향후 과제**
최근 공개된 YOLOv7 알고리즘을 적용하여 현 모델과 탐지 성능을 비교 및 성능 

1차 적용 결과 




## **ETG(EoltTeuGi)팀소개**

| 구 분 | 이 름    | 이 메 일                |
| ----- | -------- | --------------------- |
| 팀 장 | 김 선 정 | <toursun@naver.com>   |
| 팀 원 | 주 은 정 | <hahory0@naver.com>   |
| 팀 원 | 연 지 수 | <dydy11642@gmail.com> |
| 팀 원 | 이 서 영 | <zjarhk21@naver.com>  |
