학습한 Best 모델을 안드로이드 App에 적용하기 위해 Pytorch Torchscript Lite Model로 추출

YOLOv5에서 제공하는 export.py 수정 필요
*Edit export.py to make the following two changes:
After f = file.with_suffix('.torchscript.pt'), add a line fl = file.with_suffix('.torchscript.ptl') After (optimize_for_mobile(ts) if optimize else ts).save(f), add (optimize_for_mobile(ts) if optimize else ts)._save_for_lite_interpreter(str(fl))
Now run the script below to generate the optimized TorchScript lite model yolov5s.torchscript.ptl and copy it to the android-demo-app/ObjectDetection/app/src/main/assets folder (the original full JIT model yolov5s.torchscript.pt was also generated for comparison):
python export.py --weights yolov5s.pt --include torchscript
