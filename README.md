**WARNING SYSTEM FOR DRIVER**   
This repository contains code for a driver drowsiness detection system that captures videos and detects the driver's face in every frame using image processing techniques. The system employs traditional methods along with machine learning algorithms to detect driver fatigue and issue timely warnings to prevent accidents.   
This system offers a non-intrusive solution by capturing videos and analyzing facial landmarks to compute the Eye Aspect Ratio (EAR) for detecting drowsiness. Machine learning algorithms are employed to enhance the efficacy of the approach.   
**Capturing Input Video:** The input video is captured using a webcam (camera) and then extracted and converted into frames for processing.   
**Face Detection:** The system detects the driver's face in each frame, a crucial step in the processing pipeline.   
**Landmarks Prediction:** Facial landmarks, including eyes, lips, eyebrows, nose, chin, and jawline, are predicted using the 68 landmark facial feature predictors from dlib.    
**EAR and MAR Calculation:** Once the landmarks are predicted, the Eye Aspect Ratio (EAR) and Mouth Aspect Ratio (MAR) are computed using eye landmarks and mouth landmarks, respectively, to determine if the driver is drowsy.   
**Producing Warning Messages:** If the eyes are closed for more than a given time interval, the system warns the driver by playing an alarm. If the eyes are open, it displays the message "eyes open" and continues the process.   
