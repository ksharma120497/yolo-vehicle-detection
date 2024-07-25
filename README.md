# yolo-vehicle-detection
Group 4 CSCI 635-Machine Learning Project RIT Spring 2024

The primary objective of our project is to develop a system capable of detecting wrong-way driving vehicles in real-time using surveillance video data. This system leverages the You Only Look Once (YOLO) object detection algorithm in conjunction with a centroid tracking algorithm to accurately identify vehicles moving in the wrong direction. Wrong-way driving, a significant cause of road accidents and traffic congestion, poses a substantial risk to road safety. Our system aims to mitigate these risks by providing a reliable, automated monitoring tool to assist in traffic management and enforcement.


## Running the code on CS Server

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
## Output

The output will be saved in ./yolov5/runs/detect/exp{x}

https://github.com/user-attachments/assets/43aec5d4-261f-49c2-a52b-a1e956db0be1


## References

1. Redmon, J., Divvala, S., Girshick, R., & Farhadi, A. (2016). You Only Look Once: Unified, Real-Time Object Detection. Proceedings of the IEEE conference on computer vision and pattern recognition.
2. Rahman, Z., Mazumder Ami, A., & Ullah, M.A. (2020). A Real-Time Wrong-Way Vehicle Detection Based on YOLO and Centroid Tracking. Chittagong University of Engineering and Technology.
3. He, K., Gkioxari, G., Dollar, P., & Girshick, R. (2017). Mask R-CNN. 2017 IEEE International Conference on Computer Vision (ICCV).
4. Bangladesh Road Accidents in 2019 Statistics by Nirapad Sarak Chai. (2020). The Daily Star.
5. Pour-rouholamin, M., & Shaw, J. (2015). Current Practices of Safety Countermeasures for Wrong-Way Driving. TRB 94th Annual Meeting Compendium of Papers.
6. Diwan, T., Anirudh, G. & Tembhurne, J.V. Object detection using YOLO: challenges, architectural successors, datasets and applications. Multimed Tools Appl 82, 9243–9275 (2023). https://doi.org/10.1007/s11042-022-13644-y







