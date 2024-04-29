# yolo-vehicle-detection
Group 4 Machine Learning Project RIT Spring 2024

This project focuses on the YOLOv8n model which is used to detect objects. In our application, we are using this model to detect the vehicles driving on the wrong side of the road

# Running the code on CS Server

Login to the CS server through ssh and then after setting up a project location run the following command

```bash
git clone 
cd yolo-vehicle-detection
pip install -r requrirements.txt
```

We can use conda to create a different environment to run this

After everything is setup, run the below command for the inference

```bash
python3 detect_wrong.py --source overpass.mp4 --weights ./my_coco.pt --data ./data/my_coco.yaml
```

The output will be saved in ./yolov5/runs/detect/exp{x}





