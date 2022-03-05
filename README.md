# yolov5

# train model
python train.py --img 640 --cfg models/yolov5s.yaml --hyp data/hyp.scratch.yaml --batch 32 --epochs 2 --data data/custom.yaml --weights yolov5s.pt --workers 2 --name yolo_road_det

# Test detect
** เปลี่ยนพารามิเตอร์ --weights ให้ถูกโฟลเดอร์

python detect.py --source datasets/images/test/ --weights runs/train/yolo_road_det3/weights/best.pt --conf 0.25 --name yolo_road_det
