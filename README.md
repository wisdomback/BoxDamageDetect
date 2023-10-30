# ver 0.0.0

사용법 :

사전설정 :
-
cd BoxDamageDetect
pip install -r requirements.txt
pip install roboflow


학습 :
-
python3 train.py --img 416 --batch 4 --epochs 150 --data 'dataset/data.yaml' --weights yolov5s.pt


탐지 :
-
python3 detect.py --weights runs/train/exp?/weights/best.pt --img 416 --conf 0.1 --source 0
