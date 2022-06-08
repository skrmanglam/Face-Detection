# Face-Detection
This repository contains many popular face-detection algorithm and applications.

1) face detection using dlib -> This is a python code sourced from pyimage blog and uses dlib to indentify features of face(called landmarks here). dlib   uses HOG+Linear SVM & MMOD CNN in background for detection. This code currently accepts arguments via command line in terms of "--shape-predictor" which is "path to facial landmark predictor" and "--image" which is "path to input image". This gets tricky to run it via IDE like Pycharm. In next iteration I will change this behaviour to hardcode the input in script itself or use GUI libs like Tkinter to pass the filename dynamically. This code also needs dlib pretrained model to run, which can be found here : https://github.com/davisking/dlib-models/blob/master/shape_predictor_68_face_landmarks.dat.bz2.

2) facial_landmarks_dlib_webcam -> This code shows easy implemntation of dlib to classify facial features on webcam feed.

3) drowsiness_detection_dlib -> This code does drowsiness detection/eye fatigue detection. It works on dlib to extract landmarks of eyes. It then calculates EAR(eye aspect ratio){ear = (A + B) / (2.0 * C)}. Comparing it to a threshold set by user (tweakable parameter), it then detects that wether the eye has blinked or not. If both eyes blink for say 4 consecutive frames( again tweakable parameter), the algorithm says the user is drowsy and prints it on the screen.
