# Facial-Emotion-Detection
A Facial Emotion Detector using AlexNet for recognising emotions like Happy,Neutral,Sad.
This was developed as  fun stuff for the Summer Project back in 2017 with 67% Accuracy.This project also won the "Best summer Project Award" in Fr.C Rodrigues Institute Of Technology,Mumbai. 

## Dataset

We use the [FER-2013 Faces Database](http://www.socsci.ru.nl:8180/RaFD2/RaFD?p=main), a set of 28,709 pictures of people displaying 7 emotional expressions (angry, disgusted, fearful, happy, sad, surprised and neutral). 

## Steps for installation

1.create a virtual enviroment using `virtualenv`

```bash
virtualenv -p python3 ./
source ./bin/activate

```
2. install all the requirements
```bash
pip install -r requirements.txt
```

3.The data is in CSV and we need to transform it using the script `csv_to_numpy.py` that generates the image and label data in the `data` folder.

```bash
$ python3 csv_to_numpy.py
```
## Usage

```bash
# To train a model
$ python3 emotion_recognition.py train


# To use it live
$ python3 emotion_recognition.py poc
```

output:

![sample live demo](./images/demo.png)
