# TraffiKAI

A-EYE on ROADS!
An AI & ML solution to solve some of the basic but most important traffic problems in day to day life.  

Youtube Video Link: https://www.youtube.com/watch?v=xcmVi65hgkA

Problem Statement:- The increasing number of vehicles in cities can cause high volume of traffic, and implies that traffic congestion has become more critical nowadays. In addition to that, fatalities due to traffic delays of emergency vehicles such as ambulance & fire brigade is a huge problem. In daily life, we often see that emergency vehicles face difficulty in passing through traffic.

Objective:- Objective of proposed solution is to improve efficiency of existing traffic signaling system. The goal of the project is to automate the traffic signal system and make it easy for the traffic police department to monitor the traffic.

Solution:- The solution to solve the above problems as proposed are Dynamic Traffic Signaling and Emergency Vehicle Detection through both audio and video. The aim is to keep the same infrastructure and making delta changes in the system using the power of AI & ML.

https://user-images.githubusercontent.com/80829447/205123673-82164b3f-d8cd-4d97-8265-f1de680698a2.mp4

## Dynamic Traffic Signaling
Dynamic Traffic Signaling is implemented by calculating the density of traffic in each lane in a multi lane system and using this information it turns the signal lights green or red accordingly. It allocates the least time to the lane which has less density traffic and the time saved here is allocated to the lane which has high density traffic.  
Object detection alogorithm: Single Shot Detector (trained on COCO dataset)  
Teck Stack: Python, PyQT, OpenCV, Streamlit

## Emergency Vehicle Detection
Emergency Vehicle is detected by two methods in order to ensure the certainty of presence of an emergency vehicle in the input medium. The two methods include audio and video. Firstly, the video is processed frame by frame and the presence of emergency vehicles are found out and returns the confidence level and it returns a probability score.
The detection is also preformed through audio and the video's audio is passed through a CNN model which gives a probability score.
The probability scores from each models is obtained and ensemble learning is performed to get the final verdict.  
Image Classification alogorithm: DenseNet-169  
Tech Stack: Python, PyQT, OpenCV, Streamlit

System Workflow:-  

![Workflow](https://user-images.githubusercontent.com/80829447/205130227-27c7a87d-dcd4-44b2-a248-9f9dc7bbba03.jpg)

GUI:  


https://user-images.githubusercontent.com/80829447/205130444-28d5a190-54b9-424e-b6b2-5154ea2337d0.mp4

Steps to run this project:  
STEP 1: Download the models and the weights from the drive link provided below.  
STEP 2: Clone the GitHub repository.  
STEP 3: Run the code provided below in the terminal of the project folder.

Install the requirements:
```
pip install -r requirements.txt
```

Run the app:
```
streamlit run app.py
```

Drive Link: https://drive.google.com/drive/folders/1TAgqHR8HnlVbFOhKwOagTckX0T06pOVv?usp=sharing 

Collaborators:  
Mani Kanta: [https://github.com/Manikanta-7342](url)  
Akhil: [https://github.com/Akhil5347](url)  
Shreyas: [https://github.com/ShreyasKuntnal](url)





