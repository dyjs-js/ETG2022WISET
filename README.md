# 딥러닝 기반의 객체 탐지 프로젝트 : 앗! 조심해

## **개발 배경**
- 보행 중 스마트폰 사용률이 높은 가운데 안전사고의 위험성도 높음
- 인도 내 안전사고에 대해서는 적극적인 예방책이 부족함
- 추가적인 설비없이 스마트폰을 활용하여 안전사고를 줄일 수 있는 방법에 대해 고민

## **시연영상**
- Youtube URL 추가하기

## **개발환경**
![개발환경및언어](https://user-images.githubusercontent.com/85267081/188958817-1ec23f11-0ee6-4e79-b23e-f5133c0305f5.jpg)

## **System Achitecture**
딥러닝 객체 탐지 알고리즘인 YOLOv5, YOLOv7을 활용하여 이미지/영상에서 Bollard, 전동킥보드를 탐지하고 안드로이드 앱을 통해 스마트폰 사용자에게 알림
(YOLOv5, YOLOv7 : 우수한 성능과 빠른 실행 속도)

![시스템구성및아키텍쳐](https://user-images.githubusercontent.com/85267081/188958851-d922d60f-6792-43de-9026-c0ab6b20f036.jpg)

## **주요기능**
- 실시간으로 인도 내 장애물(Bollard, 전동킥보드)을 탐지하여 안드로이드 앱을 통해 스마트폰 사용자에게 알림으로써 인도 내 스마트폰 사용 보행자들의 안전사고의 발생률을 낮춤

![image](https://user-images.githubusercontent.com/85267081/188801809-139a928d-fb92-4d35-b36c-900967f592d3.png)

## **Dataset**
#### Bollard  
###### 이미지 및 좌표 정보 > AI-Hub 사이트(https://aihub.or.kr/) '인도 보행 영상' Dataset에서 추출
#### 전동킥보드 
###### 이미지 > Image crawling을 통해 구글, 네이버에서 공유킥보드 이미지 630장 + 직접 핸드폰으로 촬영한 이미지 33장
###### 좌표정보 > roboflow.com에서 1299장 직접 annotation함(Dataset명 : bolles)
            
![image](https://user-images.githubusercontent.com/85267081/188961381-b5537d43-61c6-4208-80d9-924376e0d5e6.png)

## **ETG(EoltTeuGi)팀소개**
    - 팀장 : 김선정
    - 팀원 : 주은정, 연지수, 이서영
