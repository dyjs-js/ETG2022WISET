# TO DO 

# 사용 모델 선택
  - YOLOv3 에서 YOLOv5로 변경
    > FPS(Frame Per Seconds)와 mAP(Mean Average Precision)가 높은 YOLOv5로 변경
    > 또한, 제작자의 github에서 패키지를 다운로드 받아 바로 모델을 학습하고 사용할 수 있음

# 모델을 사용하기 위한 작업(데이터 수집 및 전처리)
  - Dataset 생성 
    > AI hub에서 "인도보행 영상" dataset 확보 
      https://aihub.or.kr/aihubdata/data/view.do?currMenu=115&topMenu=100&aihubDataSe=realm&dataSetSn=189
    > "인도보행 영상-바운딩박스" image 및 xml 파일을 이용한 label 및 좌표값 parsing
    > YOLOv5 + roboflow site를 이용하여 원하는 데이터셋 생성
      (train:validation:test=7:2:1)

  - 8월 18일 데이터 전처리에 대한 처리 방법 리뷰 및 test
    > roboflow.com site
    > image(jpg) + bounding box labeling 정보(txt) 파일로 Dataset 생성

# 모델선택 및 학습
  - 8월 23일 기존 YOLOv3에서 YOLOv5+Pytorch 모델로 변경 및 테스트 코드 리뷰
    > 김선정/주은정


# 팀오프라인 일정
  - 8월 18일 목요일 오전 10시
  - 8월 23일 화요일 오전 10시


# 멘토링 일정 
  - 8월 27일 토요일 오전 10시30 오프라인 진행


# 참고사이트 
  1. Roboflow-Train_YOLOv5 https://colab.research.google.com/drive/1gDZ2xcTOgR39tGGs-EZ6i3RTs16wmzZQ
  2. https://github.com/ChelseaGH/sidewalk_prototype_AI_Hub
  3. https://github.com/ultralytics/yolov5
  4. https://blog.roboflow.com/how-to-train-yolov5-on-a-custom-dataset/
  5. https://roboflow.com/