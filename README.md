

# OverView of the Project

1. Opening background information

2. General description of the current project 

3. Proposed idea for enhancements to the project 

4. Value and significance of this project

5. Current limitations 

6. Literature review 



## 1 .Opening Background Information 

* Table tennis is one of the most popular sports worldwide, where technique and strategy play crucial roles. 
As a result, there is a growing demand for improved methods of match analysis and training.
With advancements in AI technology, the ability to analyze data and react in real time during matches has become a possibility. 
Based on this context, the aim of this project is to develop a system that uses AI to detect and analyze the movement of a table tennis ball.  

## 2. General Description of the Current Project

- The current project aims to develop a system using YOLOv5 (Object Detection Model) to detect table tennis balls in real-time.
This system analyzes footage captured by high-speed cameras to track the position and movement of the ball.
By doing so, it generates data that can be used to assess players' techniques, such as swings, serves, and other skills, providing valuable feedback during training sessions to improve performance.


## 3. Proposed Idea for Enhancements to the Project

- The strength of this project lies in leveraging the high accuracy and speed of YOLOv5, enabling real-time data analysis.
In the future, we plan to enhance the system by integrating additional machine learning algorithms to predict the trajectory of the table tennis ball and analyze match strategies.
Additionally, we will improve the user interface (UI) to make it more accessible for players and coaches, thereby increasing the system’s practicality and ease of use.

## 4. Value and Significance of This Project 

- This project has the potential to become a valuable tool for enhancing the skills of table tennis players. By leveraging AI for objective data analysis, it maximizes the efficiency of training sessions.
Additionally, the data-driven feedback system can analyze individual players’ performances and assist in developing customized training programs. 
This not only contributes to the advancement of table tennis as a sport but also expands the application possibilities of data analysis technologies in other areas.

## 5. Current Limitations 

- The current system has a few limitations. First, the accuracy of ball detection may decrease under varying lighting conditions or complex backgrounds.
Second, tracking becomes challenging when multiple balls are present simultaneously in the frame, leading to potential confusion in object detection. 
Third, there is a need to improve the real-time processing speed of the system, which may require enhancements in hardware performance to ensure efficient handling of high-speed data streams. 
Addressing these limitations will be crucial for the system’s effectiveness in practical training environments.


## 6. Literature Review

- Existing research on table tennis ball recognition primarily focuses on high-speed object detection using computer vision and deep learning models.

- YOLO Series: The YOLO (You Only Look Once) algorithm, introduced by Redmon et al., is a model capable of rapidly detecting objects in a single network pass, demonstrating high performance in real-time object recognition. The latest version, YOLOv5, further enhances speed and accuracy, making it suitable for deployment on edge devices.
Edge Computing: Edge AI platforms like the Nvidia Jetson series allow high-performance AI tasks to be performed with low power consumption, enabling real-time data processing without relying on cloud services.
Sports Data Analysis: AI-powered analysis systems have already been adopted in sports such as soccer, basketball, and tennis, where they contribute to improving player performance and strategy analysis. For sports like table tennis, which require rapid reactions, precise data collection and analysis are crucial.
References:

- Redmon, J., Farhadi, A., "YOLOv3: An Incremental Improvement", 2018.
Bochkovskiy, A., Wang, C.-Y., Liao, H.-Y. M., "YOLOv4: Optimal Speed and Accuracy of Object Detection", 2020.
Nvidia Developer Documentation on Jetson Nano/Xavier.


## Dataset acquisition process

### 1.https://universe.roboflow.com/ Go to the link

![스크린샷(29)](https://github.com/user-attachments/assets/e06a3a05-17bc-4689-a5bc-f41921570d2e)

### Find the ping pong ball dataset and download the yolov5 dataset.

![스크린샷(30)](https://github.com/user-attachments/assets/bc8e158b-64bc-4a56-8800-ed48ed153046)
![스크린샷(43)](https://github.com/user-attachments/assets/974e4c21-c8e3-41e1-88e5-3d406367d365)

### Use Google Collaboration to create code.

### 1.Google Drive integration.

### Connect to Google Drive from Google Collection.
![스크린샷(34)](https://github.com/user-attachments/assets/a7f4426b-68b5-49be-a673-c073272c07f2)


### 2. Install yolov5.
![스크린샷(47)](https://github.com/user-attachments/assets/e914556a-a768-4e79-bd89-1dfab27556cf)

### 3.Image File Management

### Creates a folder to manage image files.
![스크린샷(36)](https://github.com/user-attachments/assets/0bbb8d2e-55fb-44b8-899f-ed0b27ec426d)

### We will put the data files received from roboflow into the path accordingly.

![스크린샷(31)](https://github.com/user-attachments/assets/d7fff744-6e16-49dd-aa1f-8d72a143f434)

### You need to modify the data.yml file you received from roboflow

![스크린샷(48)](https://github.com/user-attachments/assets/a975947b-36d4-4b35-bc3a-32a154655d77)

![스크린샷(46)](https://github.com/user-attachments/assets/1684c4dc-ea7b-41a1-8a93-f866c1369c4e)
### You can put it in like the pictures above


### 4.Generates verification data.

![스크린샷(37)](https://github.com/user-attachments/assets/4f7c1df9-6864-4c13-877c-a25fbb20adca)

![스크린샷(38)](https://github.com/user-attachments/assets/59eba4c0-a985-47c6-9647-e3c4c0a34cf1)

### 5. Gets the required library.

![스크린샷(39)](https://github.com/user-attachments/assets/7b43e8ce-0892-4ec8-8a8e-1a678d8ab9c9)

![스크린샷(40)](https://github.com/user-attachments/assets/06fcbfbe-5ff1-4211-a824-c8c8571ddfb3)

### 6. Let them learn

![스크린샷(41)](https://github.com/user-attachments/assets/806bdfbf-6bf8-429b-8869-2ac7a289e62e)

### 7. learning outcome

![스크린샷(17)](https://github.com/user-attachments/assets/3f26ff60-6aae-4fe4-8c6c-fd8a33bd2f80)

![스크린샷(18)](https://github.com/user-attachments/assets/2b57f3cd-7c9a-415a-847a-7cc58ff941d3)

![스크린샷(19)](https://github.com/user-attachments/assets/2f58aa1c-e583-4363-95f7-a53c88abe2a8)

![스크린샷(20)](https://github.com/user-attachments/assets/f303af50-2c19-470d-a142-4628be8268e1)

![스크린샷(21)](https://github.com/user-attachments/assets/68f990c1-0f71-44bf-af2a-01e310d1a837)


### 8. Validate model results
python detect.py --weight runs/train/exp/weights/best.pt --source [Path of the image to be tested] --img 640 --conf 0.8


