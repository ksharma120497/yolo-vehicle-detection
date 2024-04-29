# yolo-vehicle-detection
Group 4 Machine Learning Project RIT Spring 2024

This project focuses on the YOLOv8n model which is used to detect objects. In our application, we are using this model to detect the vehicles driving on the wrong side of the road

# Running the code on CS Server

Login to the CS server through ssh and then after setting up a project location run the following command

```bash
git clone https://github.com/ksharma120497/yolo-vehicle-detection.git
cd yolo-vehicle-detection
pip install -r requirements.txt
```

NOTE: Installation of the libraries from requirements.txt will take around 10 mins for the first time

We can use conda to create a different environment to run this

Download our best trained YOLO model from this lin
```bash
https://drive.google.com/file/d/15bjI8V68K9CACM_W2VueE0VPuio5iH7X/view?usp=share_link
```

Place this file in the root folder before running the inference


After everything is setup, run the below command for the inference

```bash
python3 detect_wrong.py --source overpass.mp4 --weights ./my_coco.pt --data ./my_coco.yaml
```

The output will be saved in ./yolov5/runs/detect/exp{x}





