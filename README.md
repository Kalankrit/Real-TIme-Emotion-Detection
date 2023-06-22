# Real-TIme-Emotion-Detection  
### Introduction  
This project aims to classify the emotion on a person's face into one of seven categories, using deep convolutional neural networks. The model is trained on the FER-2013 dataset which was published on International Conference on Machine Learning (ICML). This dataset consists of 35887 grayscale, 48x48 sized face images with seven emotions - angry, disgusted, fearful, happy, neutral, sad and surprised.

### Basic Usage  
The repository is currently compatible with tensorflow-2.0 and makes use of the Keras API using the tensorflow.keras library.

### Packages need to be installed
- pip install numpy
- pip install opencv-python
- pip install keras
- pip3 install --upgrade tensorflow
- pip install pillow

### Download FER2013 dataset
- from below link and put in data folder under your project directory
- https://www.kaggle.com/msambare/fer2013

### Train Emotion detector
- with all face expression images in the FER2013 Dataset
- command --> python TranEmotionDetector.py

It will take several hours depends on your processor. (On i7 processor with 16 GB RAM it took me around 4 hours)
after Training , you will find the trained model structure and weights are stored in your project directory.
emotion_model.json
emotion_model.h5

copy these two files create model folder in your project directory and paste it.

### Run your emotion detection test file
python TestEmotionDetector.py

### Pre-trained model  
If you do not want to train the model you can simply run the TestEmotionDetector.py without using TrainEmotionDetector.py

If you want to detect emotions in a video you can comment line 19 in TestEmotionDetector.py and uncomment line 23 and add the path of the video file.
