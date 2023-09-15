# satellite-infrastructure-detectron2

I wanted to create a basic transfer learning object detection model (based on detectron2 architecture) which will help to analyze/detect urban infrastructure (like airports, railways, cargo ports etc.) based on satellite image data.
The dataset includes satellite images aggregate from https://earth.google.com/. The COCO format dataset was created with the help of https://www.robots.ox.ac.uk/~vgg/software/via/. 

The dataset contains 140 images in png format with size 850 by 850 pixels. The train set mostly contains satellite images from Asia and Oceania (only Australia and New Zealand), while the test set contains satellite images from the Nordic region countries and Canada. 
The recent detectron2 version was trained to recognise only “airport” class to prove the potential of the model to detect objects on satellite images. As can be seen in detectron2_infrastructure_detection.ipynb file, the model successfully recognises bigger (international) airports, although the performance on satellite images with smaller (rural) airports can definitely be improved. 
