# yolov5

# train model
python train.py --img 640 --cfg models/yolov5s.yaml --hyp data/hyp.scratch.yaml --batch 32 --epochs 2 --data data/custom.yaml --weights yolov5s.pt --workers 2 --name yolo_road_det
