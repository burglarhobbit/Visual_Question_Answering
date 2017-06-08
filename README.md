# Visual_Question_Answering

This is a simple "updated" Demo of Visual Question Answering by [VQA_Demo](https://github.com/iamaaditya/VQA_Demo/) which uses pretrained models (see [VGG16](https://keras.io/applications/#vgg16) and models/VQA) to answer a given question about the given image.

## Dependency

1. Keras version 2.0.4
   * Modular deep learning library based on python

2. Tensorflow 
    * For the development of this project, I used Tensorflow 1.1.0

3. scikit-learn
   * Quintessential machine library for python

4. Spacy version 1.8.2
    * Used to load Glove vectors (word2vec)
    * You may have to upgrade your Spacy to use Glove vectors (default is Goldberg Word2Vec)
    * To upgrade & install Glove Vectors
      * pip install spacy
      * python -m spacy download en

5. OpenCV 
    * OpenCV is used only to resize the image and change the color channels,
    * You may use other libraries as long as you can pass a 224x224 BGR Image (NOTE: BGR and not RGB)

6. VGG 16 Pretrained Weights
    * Please download the weights file [vgg16_weights.h5](https://drive.google.com/file/d/0Bz7KyqmuGsilT0J5dmRCM0ROVHc/view)

## Usage

> python demo.py

Put your test images in the dataset/ directory

Expected Output:
095.2 %  train
00.67 %  subway
00.54 %  mcdonald's
00.38 %  bus
00.33 %  train station
