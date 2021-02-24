# QR code scanner
A simple Android application that decodes QR codes in the absence of one of the finder patterns.
15 neural networks are used to decode a maximum of 15 characters of the string encoded in the QR code.

## Networks Architecture
each network is composed of:
1) 625 input neurons (input qr codes have 25x25 resolution)
2) a hidden layer with 128 neurons
3) 30 output neurons (1 neurons for each character that networks can predict)

<img src="net_arch.JPG" width="25%" height="25%">

## Android application

## Citations
Model: [YOLOv3](https://pjreddie.com/darknet/yolo/)

Similar app used to develop this application: [YOLOv3-CoreML](https://github.com/Ma-Dan/YOLOv3-CoreML)

## Useful Google Colab file

[From YOLOv3 to Custom Object Detection](https://colab.research.google.com/drive/1BNajhZAxU_8J8DoK43y2JEJog0l4Hb6X)

## Before Building the App
Download the [model](https://github.com/danielecolautti/LALakersAI/tree/main/zippedModel) and copy it into LALakersAI/Utils/

## Example Images

### Model Output

<img src="images/00200_y.jpg" width="75%" height="75%">

### Live Detection

<img src="images/detection.PNG" width="25%" height="25%">

### Statistics

<img src="images/statistics.PNG" width="25%" height="25%">

### Line Up

<img src="images/lineUp.PNG" width="25%" height="25%">

### Successful Shot by Anthony Davis

<img src="images/davis.PNG" width="25%" height="25%">

### Settings

<img src="images/settings.PNG" width="25%" height="25%">
