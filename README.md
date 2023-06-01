# Hppymonk.AI
Deep Learning ANN

The MNIST dataset is a widely used benchmark dataset in the field of machine learning and computer vision. It stands for the Modified National Institute of Standards and Technology database. The dataset consists of a large collection of 28x28 grayscale images of handwritten digits (0 to 9) along with their corresponding labels.

The MNIST dataset is often used as a starting point for learning and implementing image classification algorithms. It has become a standard reference for evaluating the performance of machine learning models, particularly in the area of deep learning. Despite its simplicity compared to real-world datasets, the MNIST dataset still poses challenges due to variations in writing style, stroke thickness, and orientation.


Technologies used for  develop and implement the assignment.

Python is widely used in this project due to its extensive library and framework.
Scikit learn is used for wide range of algorithms and  tools for classification task. I used  scikitlearn libraries for the evaluation matrix.
Matplotlib are used for creating visualizations and plot graphs.
Keras is used  because it’s offers a user-friendly and flexible interface, supports various deep learning applications, and has a strong community and ecosystem, making it a popular choice for deep learning projects.

Data Set
Size and Structure: The MNIST dataset contains 60,000 training images and 10,000 testing images.
These images are evenly split into 10 classes, representing the digits from 0 to 9.
Each image is a 28x28-pixel grayscale image, meaning it has a resolution of 28 pixels in height and 28 pixels in width.
The MNIST dataset is often used as a benchmark for evaluating and comparing the performance of machine learning and deep learning algorithms, especially for tasks like image classification. It provides a relatively simple and well-defined problem domain for testing algorithms and models.


To solve an assignment using the MNIST dataset with an Artificial Neural Network (ANN), steps are as  follows:

Step 1 : Load MNIST for kersa library library
Step 2: Split the dataset into training and testing sets.
Step 3: Preprocess the data by normalizing the pixel values to a range between 0 and 1 and reshaping the input images .
Maximum pixels range is 256 so we divide each pixels value with 256 so we gate maximum value as 1.
Ste 4 : With the help of Keras Decide on the architecture of  ANN, including the number and size of layers, activation functions, and the number of neurons in each layer. For the MNIST dataset, a common choice is a feed forward neural network with multiple hidden layers.
Step 5: Initialize and Train the ANN: Initialize your ANN model with the chosen architecture. Compile the model by specifying the loss function, optimizer, and metrics to be used. Train the model using the training set by feeding the input images and their corresponding labels to the model.
Step 6: Evaluate the Model: Evaluate the trained model using the testing set. Feed the input images from the testing set to the model and compare the predicted labels with the true labels. Calculate metrics such as accuracy, precision, recall, and F1-score to assess the performance of the model.

After Evaluate the Model I do some experiment to find best no of node, layers , best optimizer and best 
Activation function best on data set using hypermeter tuning with keras library.

Step 1 : Best optimizer for MNIST data set is >>{'optimizer': 'rmsprop'}
Step 2 : Right number of nureon is >> {'units': 340}
Steps 3: Right numbe of  hidden layer is >> {'num_layers': 2}
Steps 4: Best Activation Function is 'activation1': 'relu', for hidden layer 'activation0': 'softmax', for outer layer.


