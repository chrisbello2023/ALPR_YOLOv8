# Liecense-Plate-Recognition-YOLO v8
## Demo


https://github.com/Muhammad-Zeerak-Khan/Automatic-License-Plate-Recognition-using-YOLOv8/assets/79400407/1af57131-3ada-470a-b798-95fff00254e6



## Model

A Yolov8 pre-trained model (YOLOv8n) was used to detect vehicles.

A licensed plate detector was used to detect license plates. The model was trained with Yolov8 using [this dataset](https://universe.roboflow.com/roboflow-universe-projects/license-plate-recognition-rxg4e/dataset/4). 
- The model is available [here]https://drive.google.com/file/d/11ZG1pXRz3mjJCHpxDID_b7R9Xvr3jRJD/view?usp=drive_link
  
## Dependencies

The sort module needs to be downloaded from [this repository](https://github.com/abewley/sort).

## Project Setup

* Make an environment with python=3.8 using the following command 
``` bash
conda create --prefix ./env python==3.8 -y
```

* Install the project dependencies using the following command 
```bash
pip install -r requirements.txt
```
* Run main.py with the sample video file to generate the test.csv file 
``` python
python main.py
```
* Run the add_missing_data.py file for interpolation of values to match up for the missing frames and smooth output.
```python
python add_missing_data.py
```

* Finally run the visualize.py passing in the interpolated csv files and hence obtaining a smooth output for license plate detection.
```python
python visualize.py
```
