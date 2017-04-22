# Image-Classification-Using-Random-Forest
Image Classification Using Random Forest model with K means clusttering


### Procedure Followed:

![Image](https://github.com/nandanamudi/Bigdata-Spring2017-Lab_Assignments/blob/master/Lab5/Documentation/Document%201%20(2).jpg)

**1. Splitting the input and feeding the data(70-30) as input to train.**
**2. Using the training data [Key Descriptors](https://github.com/nandanamudi/Bigdata-Spring2017-Lab_Assignments/blob/master/Lab5/Source/image_classification/src/main/scala/Descriptors_extraction.scala) are generated.**

![Image](https://github.com/nandanamudi/Bigdata-Spring2017-Lab_Assignments/blob/master/Lab5/Documentation/Images/112.PNG)

**3. Features Vectors are generated and by using [K-means clusters](https://github.com/nandanamudi/Bigdata-Spring2017-Lab_Assignments/blob/master/Lab5/Source/image_classification/src/main/scala/K_means.scala) are generated**
![Image](https://github.com/nandanamudi/Bigdata-Spring2017-Lab_Assignments/blob/master/Lab5/Documentation/Images/1.PNG)
![Image](https://github.com/nandanamudi/Bigdata-Spring2017-Lab_Assignments/blob/master/Lab5/Documentation/Images/2.PNG)

**4. Using Bag of words [histograms ](https://github.com/nandanamudi/Bigdata-Spring2017-Lab_Assignments/blob/master/Lab5/Source/image_classification/src/main/scala/Classification_main.scala#L103)are generated**
![Image](https://github.com/nandanamudi/Bigdata-Spring2017-Lab_Assignments/blob/master/Lab5/Documentation/Images/4.PNG)
![Image](https://github.com/nandanamudi/Bigdata-Spring2017-Lab_Assignments/blob/master/Lab5/Documentation/Images/5.PNG)

**5. The [histogram data is fed to the Random forest](https://github.com/nandanamudi/Bigdata-Spring2017-Lab_Assignments/blob/master/Lab5/Source/image_classification/src/main/scala/Random_forest_model.scala#L22) and a training [model](https://github.com/nandanamudi/Bigdata-Spring2017-Lab_Assignments/blob/master/Lab5/Source/image_classification/src/main/scala/Random_forest_model.scala#L103) is generated from the training data.**

![Image](https://github.com/nandanamudi/Bigdata-Spring2017-Lab_Assignments/blob/master/Lab5/Documentation/Images/7.PNG)

**6. This[ random forest model is used on the test data](https://github.com/nandanamudi/Bigdata-Spring2017-Lab_Assignments/blob/master/Lab5/Source/image_classification/src/main/scala/Classification_main.scala#L62) to predict the input test images classes.**

![Image](https://github.com/nandanamudi/Bigdata-Spring2017-Lab_Assignments/blob/master/Lab5/Documentation/Images/8.PNG)
![Image](https://github.com/nandanamudi/Bigdata-Spring2017-Lab_Assignments/blob/master/Lab5/Documentation/Images/9.PNG)
![Image](https://github.com/nandanamudi/Bigdata-Spring2017-Lab_Assignments/blob/master/Lab5/Documentation/Images/10.PNG)

## Result:

### Accuracy:
![Image](https://github.com/nandanamudi/Bigdata-Spring2017-Lab_Assignments/blob/master/Lab5/Documentation/Images/12.PNG)

### Confusion matrix:
![Image](https://github.com/nandanamudi/Bigdata-Spring2017-Lab_Assignments/blob/master/Lab5/Documentation/Images/13.PNG)

***
***


## Task 2: Client Application Using Spark API
***
Data Set Considered:
[ 4 different Categories](https://github.com/nandanamudi/Bigdata-Spring2017-Lab_Assignments/tree/master/Lab5/Source/image_classification/data/train) of Images which contains animals, buildings, statues and humans in different classes.

Created a client as a web application which makes a [call to the server]([call to the server](https://github.com/nandanamudi/Bigdata-Spring2017-Lab_Assignments/blob/master/Lab5/Source/image_classification/src/main/scala/SimpleServer.scala#L36)) with an image to be classified with all created model


Prediction image is read and [sent as test input to the Random Forest Model](https://github.com/nandanamudi/Bigdata-Spring2017-Lab_Assignments/blob/master/Lab5/Source/image_classification/src/main/scala/Predict.scala)

The Server ran and the client application connection to the server is established.
![Image](https://github.com/nandanamudi/Bigdata-Spring2017-Lab_Assignments/blob/master/Lab5/Documentation/Images1/8.PNG)


### Results:

**First Selection:**
![Image](https://github.com/nandanamudi/Bigdata-Spring2017-Lab_Assignments/blob/master/Lab5/Documentation/Images1/1.PNG)

**Image Histogram**
![Image](https://github.com/nandanamudi/Bigdata-Spring2017-Lab_Assignments/blob/master/Lab5/Documentation/Images1/6.PNG)

**Response**
![Image](https://github.com/nandanamudi/Bigdata-Spring2017-Lab_Assignments/blob/master/Lab5/Documentation/Images1/7.PNG)


**Second Selection:**
![Image](https://github.com/nandanamudi/Bigdata-Spring2017-Lab_Assignments/blob/master/Lab5/Documentation/Images1/2.PNG)

**Image Histogram**
![Image](https://github.com/nandanamudi/Bigdata-Spring2017-Lab_Assignments/blob/master/Lab5/Documentation/Images1/4.PNG)

**Response**
![Image](https://github.com/nandanamudi/Bigdata-Spring2017-Lab_Assignments/blob/master/Lab5/Documentation/Images1/5.PNG)


**Third Selection:**
![Image](https://github.com/nandanamudi/Bigdata-Spring2017-Lab_Assignments/blob/master/Lab5/Documentation/Images1/3.PNG)


***
***


## Task 3: Google Conversions Action API
***
**An Agent with the name Envisager is created here.**
![Image](https://github.com/nandanamudi/Bigdata-Spring2017-Lab_Assignments/blob/master/Lab5/Documentation/Images2/11.PNG)



**Welcome Intent and few other intents were created.**
![Image](https://github.com/nandanamudi/Bigdata-Spring2017-Lab_Assignments/blob/master/Lab5/Documentation/Images2/19.PNG)



**Entities were created to identify with different names**
![Image](https://github.com/nandanamudi/Bigdata-Spring2017-Lab_Assignments/blob/master/Lab5/Documentation/Images2/20.PNG)



**User queries were added**
![Image](https://github.com/nandanamudi/Bigdata-Spring2017-Lab_Assignments/blob/master/Lab5/Documentation/Images2/12.PNG)



**Responses to the user queries were written**
![Image](https://github.com/nandanamudi/Bigdata-Spring2017-Lab_Assignments/blob/master/Lab5/Documentation/Images2/13.PNG)



**Few other queries in different intents were written**
![Image](https://github.com/nandanamudi/Bigdata-Spring2017-Lab_Assignments/blob/master/Lab5/Documentation/Images2/14.PNG)



**Responses and Image Content is added for the user responses**
![Image](https://github.com/nandanamudi/Bigdata-Spring2017-Lab_Assignments/blob/master/Lab5/Documentation/Images2/15.PNG)



**Query Responses in the Api.ai**
![Image](https://github.com/nandanamudi/Bigdata-Spring2017-Lab_Assignments/blob/master/Lab5/Documentation/Images2/6.PNG)



**The agent is integrated and deployed**
![Image](https://github.com/nandanamudi/Bigdata-Spring2017-Lab_Assignments/blob/master/Lab5/Documentation/Images2/10.PNG)



**Response in the web simulator**
![Image](https://github.com/nandanamudi/Bigdata-Spring2017-Lab_Assignments/blob/master/Lab5/Documentation/Images2/16.PNG)



**Response in json format**
![Image](https://github.com/nandanamudi/Bigdata-Spring2017-Lab_Assignments/blob/master/Lab5/Documentation/Images2/18.PNG)



**Other Query**
![Image](https://github.com/nandanamudi/Bigdata-Spring2017-Lab_Assignments/blob/master/Lab5/Documentation/Images2/9.PNG)



**Few Requests history**
![Image](https://github.com/nandanamudi/Bigdata-Spring2017-Lab_Assignments/blob/master/Lab5/Documentation/Images2/17.PNG)



***
***


