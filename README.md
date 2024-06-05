#Dataset Source
https://universe.roboflow.com/roboflow-universe-projects/fall-detection-ca3o8/dataset/4

#Train
python train.py --img-size 640 --batch-size 16 --epochs 10 --data data/data.yaml --cfg models/yolov5s.yaml --name fall_detection

#Test
python detect.py --weights runs/train/fall_detection/weights/best.pt --source fall.jpg --imgsz 640

I got the 86% accuracy in detecting falls of human using fall detection image dataset in yolov5.