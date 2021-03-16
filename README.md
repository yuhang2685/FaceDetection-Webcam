# FaceDetection-Webcam

[![license](https://img.shields.io/github/license/mashape/apistatus.svg)](LICENSE)

## Introduction
The work is originally created by https://github.com/theAIGuysCode/colab-webcam.
Running in Google Colab, it applies OpenCV's Haar Cascade for face detection in webcam image and video.

The advantege for using Haar Cascade for object detection is handy, 
the disadvantege is not supporting for customization.

## Working Mechanism
Once the image is ready, 
it is first converted into gray image for faster detection.
Then Haar Cascade is applied on the image, 
and the bounding boxes are drawn on the image.

For videos, we obtain boxes from the previous frame and draw them on a blank image, 
then overlay the image on the next frame.

Since Colab is running in cloud VM, 
we have to use Javascript to connect Colab with local webcam.


## Reference
- [colab-webcam](https://github.com/theAIGuysCode/colab-webcam) by [The AI Guy](https://github.com/theAIGuysCode).

- [Browser-based Models with TensorFlow.js](https://www.coursera.org/learn/browser-based-models-tensorflow?specialization=tensorflow-data-and-deployment) by [Laurence Moroney](https://www.coursera.org/instructor/lmoroney) and [DeepLearning.AI](https://www.deeplearning.ai/).

