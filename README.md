# Sleep-Apnea-Detection-using-ECG-Signal


**Project Description: -**
      
    Detect Sleep Apnea using ML and Mobile Application.


**Requirements: -**

    • AD8232 ECG Monitor Sensor Module
    • Android App
    • WIFI Module
    • Smartphone
    • Jumper Cables


**Key Components of Project: -**

    • Google Colab (Cloud): -
         Project on which we are working contains dataset of size 400MB having .csv
         Extension. To training these kinds of data on local machine is not possible because it needs a
         lot of computing power. Though I have tried it and my machine got hanged. That’s why I
         switched to Cloud (Google Colab)
         
    • AD8232 ECG Monitor Sensor Module
         This module can be used to detect and record ECG Data of patient which we need to
         detect weather that patient has sleep apnea or not
         
    • WIFI Module
         Data that we recorded has to be sent on cloud for prediction of Sleep Apnea for that
         purpose we need WIFI module using which we can send data on cloud.
         
    • Android App
         Whatever data that ECG Sensor has recorded can be send on cloud through Mobile
         app and also its result can be seen on mobile.



**High Level Design: -**

<p align="center">
 <img  src="https://github.com/sanket9006/Sleep-Apnea-Detection-using-ECG-Signal/blob/master/Flow.png">
</p>



      First ECG Sensor is attached to patient body and all readings are Recorded and transferred
      on cloud with the help of WIFI module. Once data is loaded onto cloud to our machine learning this
      data is fetched as input and as a result it will predict weather the patient has sleep apnea or not.
      Once the result is known (calculated) it is uploaded on to mobile.
      
 
**Low Level Design: -**

      In this project we will detect Sleep Apnea Detection using machine learning. We have two
      files main.py, splitdata.py, dataVisualization.py. splitdata.py file is python 3.7 file used to split raw
      sleep apnea ECG data into python array and store it in ApneaData.pkl. Main.py is main file where
      machine learning algorithms are implemented. dataVisualization.py graphically plots the data by
      using dimensionality reduction techniques.
      
      Datasets
      
      Sleep Apnea dataset consists of around 16000 people ECG data sampled at 6000 sample
      points each and 1 or 0 representing whether person have sleep Apnea or not. Data set structure
      looks like
      
      [
      [0,1,2,.....,6000,cls],
      [0,1,2,.....,6000,cls],
      [0,1,2,.....,6000,cls],
      ...
      ...
      ...
      ..
      [0,1,2,.....,6000,cls]
      ]
      
      cls maybe 0 or 1. 1 represents Apnea and 0 represents non Apnea    

      Algorithms
            The algorithm we are using is ensemble.RandomForestClassifier from sklearn which is faster
            and more accurate. This algoritm is picked and tested with few other comparison. Feel free to
            change other algorithm classifier(clf) from sklearn.
            Using T-distributed Stochastic Neighbor Embedding algorithm to visualize data.
      
      

<p align="center">
 <img  src="https://github.com/sanket9006/Developer-Student-Clubs-DSC-Solution-Challenge-2020/blob/master/code.png">
</p>

**High Level Design: -**

**High Level Design: -**

