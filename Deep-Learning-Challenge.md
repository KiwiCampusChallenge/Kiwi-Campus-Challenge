# Deep Learning Challenge

The following tasks are designed to test your current skills. Some of the tasks may be easier than others; moreover, some tasks will require skills that you will acquire in the Self-dringving Cars nanodegree, so do not feel bad if you decide your not ready to perform some of the tasks.

**Task 1 (5 points)**

1. Create a *GitHub* ([https://github.com/](https://github.com/)) repository and name it "German Traffic Signs Detector".
2. Create an [app.py](http://application.py) file, which will store a *Click* application ([http://click.pocoo.org/5/](http://click.pocoo.org/5/)); this will be the main program, and you will implement several groups ([http://click.pocoo.org/5/commands/](http://click.pocoo.org/5/commands/)), which are related to the rest of the tasks of this challenge. 
3. Create directories with the following structure:
```
      German Traffic Signs Detector
      	|
      	|-images/
      			|-train/
      			|-test/
      			|-user/
      	|-reports/
      			|-model1.ipynb
      			|-model2.ipynb
      			.
      			.
      			.
      	|-models/
      			|-model1/
      				|-README.md
      				|-saved/
      			|-model2/
      				|-README.md
      				|-saved/
      			.
      			.
      			.
      	|-README.md
      	|-app.py
```
**Task 2 (15 points)** 

Create a *download* group that will download all data from the *German Traffic Signs Dataset* ([http://benchmark.ini.rub.de/?section=gtsdb&subsection=dataset](http://benchmark.ini.rub.de/?section=gtsdb&subsection=dataset)). This will store the the data set inside an *images* folder.

Since you only need to build CLASSIFICATION models, please ignore all images related to object detection (the best solution would be to ignore them from code).

The train folder will contain images for training the models; the test folder will have images on which you will validate your models; and finally, the user folder should be created by you but left empty, we will put our own images there to make our own tests on your code. 

From the total of the images in the data set, leave 80% for training and 20% for testings your models.

The program should be executed as follows:

    python app.py download

**Task 3 (15 points)**  

Create, train and save a logistic regression model using scikit-learn ([http://scikit-learn.org/stable/](http://scikit-learn.org/stable/)). 

**Task 4 (20 points)**

Create, train and save a logistic regression model using TensorFlow ([https://www.tensorflow.org/](https://www.tensorflow.org/))

**Task 5 (35 points)**

Create, train and save a LeNet model ([http://yann.lecun.com/exdb/publis/pdf/lecun-01a.pdf](http://yann.lecun.com/exdb/publis/pdf/lecun-01a.pdf)) in Tensorflow. 

**Task 6 (10 points)**

Create an application that will use a chosen model and run inference on images saved in a particular directory. For each image in such directory you should show a window with the image together with its label. It should be executed as follows:

    python app.py infer -m [chosen model] -d [directory with user data]

**Further notes:**

Task 3,4,5 should be executed as follows:

    python app.py train -m [chosen model] -d [directory with trainig data]

    python app.py test -m [chosen model] -d [directory with test data]

Each of the previous two commands should output the accuracy of your model.

You can use hyperparameter tunning, dimensionality reduction and regularization techniques with any model.

For every model you implement (tasks 3, 4 and 5) you should include a description of the model in a [READM](http://readm.md)[E[.md](http://readm.md) inside that model's directory. Also, you must write a report for each of the models, which will take the model saved from models/model1/saved/ 

It is very important that you implement and train the models in TensorFlow (tasks 4 and 5) from scratch. DO NOT use someone's else model. In fact, the description of the model of task 5 should reflect what the authors of the paper have proposed.

You DO NOT have to implement all models, we do not really expect you to do so, we encourage you to try with the simplest model and start building up complexity. In fact the different tasks are not mandatory, but they will give you points.

It is a requirement that you use good programming style, think of functions, clases, docstrings, etc.

DO NOT include the images in the directory

