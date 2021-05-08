# PR-Project
                                  Sign Language Alphabet Recognition using ANN and CNN
1. Motivation
American Sign Language (ASL) is a natural language with the same linguistic characteristics as spoken languages, with grammar that is different from the English language. Movements of the hands and face show ASL. It is the primary language of many North Americans who are deaf and have difficulty hearing and is used by some hearing people. It plays an essential role in the life of people who have impaired hearing and speaking inabilities. American Sign Language (ASL) alphabet recognition with computer vision is a very challenging task because of the complexity in ASL signs, high inter-class similarities, constant occlusions, and large intraclass variations. Sign language recognition will make communication more comfortable if one person is not well-versed with the language.
Problem Statement
During recent years a large number of computer aided applications have been developed to help the disabled people. This has improved the communication gap between the able and the hearing-impaired community. An intelligent signed alphabet recognizer can work as an aiding agent to translate the signs to words (and also sentences) and vice versa. Our goal is to develop a signed alphabet recognizer using Convolutional Neural Network.
2. Data Acquisition
Data acquisition is one step of the sign language recognition, this step consists of digitize the information from the user to make it usable to classification algorithms, the information from the user can be acquired in different ways depending on the tools used, such as visual based like cameras or wearable like the use of electromyogram, sensors in a glove, etc. Those tools have different advantages such as low-cost, hardware and software compatibility, user detection, etc., in the same way those tools have disadvantages such as occlusion, cost, trouble with the users, etc. Depending on the scope of the research the tools to obtain information from the user can change.
3. Data preprocessing
For making the dataset suitable to perform various algorithms to predict sign language alphabet labels correctly, we will visualize our dataset to see if it is balanced or not. We will also store the labels of each image which is mapping with their respective labels in a list and generate a random image to perform class label verification. We will also perform normalization so that our model works effectively.
4. Proposed Methodology
4.1 Dataset Collection
For our project we use the dataset available on the Kaggle – https://www.kaggle.com/grassknoted/asl-alphabet
The training data set contains 87,000 images which are 200x200 pixels. There are 29 classes, of which 26 are for the letters A-Z and 3 classes for SPACE, DELETE and NOTHING. These 3 classes are very helpful in real time applications, and classification. The test data set contains a mere 29 images, to encourage the use of real-world test images.
Fig 1.
4.2 Model Construction and Validation
Our approach to building this Sign Language Alphabet Recognizer model is discussed in four steps:
1. Explore the dataset
2. Build a CNN model
3. Train and validate the model
4. Test the model with test dataset
4.3 Language and Technology used
We will use Python 3 computer language in our project. With the help of the OS module, we will iterate over all the classes and append images and their respective labels in the data and labels list. The PIL library is used to open image content into an array. From the keras.utils package, we will use to_categorical method to convert the labels present in the list into one-hot encoding(One hot encoding is a process by which categorical variables are converted into a form that could be provided to ML algorithms to do a better job in prediction).We will need to convert the list into numpy arrays for feeding to the model.
4.4 Description of ML Algorithm to be used (Techniques)
To classify the images into their respective categories, we will build a CNN model (Convolutional Neural Network). CNN is best for image classification purposes. The name “convolutional neural network” indicates that the network employs a mathematical operation called convolution. Convolution is a specialized kind of linear operation. Convolutional networks are simply neural networks that use convolution in place of general matrix multiplication in at least one of their layers. There are no recurrent connections in CNN. A convolutional neural network consists of an input and an output layer, as well as multiple hidden layers. The hidden layers of a CNN typically consist of a series of convolutional layers that convolve with a multiplication or other dot product. The activation function is commonly a RELU layer, and is subsequently followed by additional convolutions such as pooling layers, fully connected layers and normalization layers, referred to as hidden layers because their inputs and outputs are masked by the activation function and final convolution.
Artificial Neural Networks (ANN) are information processing architecture, which are loosely modelled on the brain. They consist of a large number of interconnected processing units (neurons). ANN is a parallel computational system consisting of many simple processing elements connected together in a specific way in order to perform a particular task. They are generally used to model relationships between inputs and outputs or find patterns in data.
5. Evaluation Metrics
For Evaluating our model, the performance measures we are using to evaluate our models are: Accuracy, Precision, Recall, F1 Score and AUC Score.
6. Deliverables
There will be 3 deliverables that are Research Paper, Presentation and Trained Model.
