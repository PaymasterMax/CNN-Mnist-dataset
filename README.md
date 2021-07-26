# CNN-Mnist-dataset

1. The dataset used here is the mnist dataset found in tf.keras.datasets.mnist.load_data()
2. This dataset contains images of handwritten digits 
3. In this model, Convulated neural network and maxpooling has been employed to perform picking out the important features of the dataset
4. The model (CNN models) are stacked om top of the models before the hidden layers added later on it.
5. The dataset is preprocessed by default, all we have to do is simply reshaping the images to the 4 dimensions expected by the convulation models. then feed it to the hidden layers of the network.
6. The CNN networks are not surfficient to do the image classification by their own, they depend on the hidden dense network. 
7. The dataset contains 60k training labeled images, and 10k test / validation images.
8. The sequential model is composed of 2 hidden layers and the output model which contains 10 neurons.

9. Model was compiled using the following parameters: 
      
        i) metrics - accuracy
        ii) loss function - sparse_categorical_crossentropy
        iii) batch_size 32
        iv) Epoch of 4 is enough to prevent overfit.
        v) The optimizer used was adam, but ofcourse we had other options.
        
  
 
 
 # Analysis
 The model initially had a higher loss and slighly lower accuracy score just before using cnn.
The model trained on the mnist data.
It scored an average of 99.58% on training data and 98.28% on test data,
The loss computed was roughly  0.02% .
