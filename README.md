# Face-Detection
This repository contains many popular face-detection algorithm and applications.

1) face detection using dlib -> This is a python code sourced from pyimage blog and uses dlib to indentify features of face(called landmarks here). dlib   uses HOG+Linear SVM & MMOD CNN in background for detection. This code currently accepts arguments via command line in terms of "--shape-predictor" which is "path to facial landmark predictor" and "--image" which is "path to input image". This gets tricky to run it via IDE like Pycharm. In next iteration I will change this behaviour to hardcode the input in script itself or use GUI libs like Tkinter to pass the filename dynamically. This code also needs dlib pretrained model to run, which can be found here : https://github.com/davisking/dlib-models/blob/master/shape_predictor_68_face_landmarks.dat.bz2.

2) facial_landmarks_dlib_webcam -> This code shows easy implemntation of dlib to classify facial features on webcam feed.
