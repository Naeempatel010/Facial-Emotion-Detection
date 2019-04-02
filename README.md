# Facial-Emotion-Detection
A Facial Emotion Detector using AlexNet for recognising emotions like Happy,Neutral,Sad.Developed for the Summer Project Way back in 2017 with 67% Accuracy


## Dataset

We use the [FER-2013 Faces Database](http://www.socsci.ru.nl:8180/RaFD2/RaFD?p=main), a set of 28,709 pictures of people displaying 7 emotional expressions (angry, disgusted, fearful, happy, sad, surprised and neutral). 

Install all the dependencies using `virtualenv`.

```bash
virtualenv -p python3 ./
source ./bin/activate
pip install -r requirements.txt
```

The data is in CSV and we need to transform it using the script `csv_to_numpy.py` that generates the image and label data in the `data` folder.

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


