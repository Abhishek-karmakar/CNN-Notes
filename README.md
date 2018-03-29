## CNN - Convolutional Neural Network - notes
---------------------------------------------

(Intuition)

1.> What are convolutional Neural Network
2.> Step - 1. Convolutional Operation. Feature Detectors, Features Maps.  
2.> Step - 1b. ReLU Layer
3.> Step - 2.  Pooling. 
4.> Step - 3. Flattering
5.> Step - 4. Full Connection 
6.> Summary

TODO : for later , Softmax and Cross-Entropy.

1.> What are convolutional Neural Networks
 
The following steps are processed. 
 Convolution
 Max Operation. 
 Flattening
 Full Connection. 

 Convolution function
 ---------------------
 Is a combined integration of two functions and it shown how one function modifies the shape of the other. 
 There is a feature detector or filter , which is a matrix of pixel, multiply this with a previous image so that 
 Image on the right - Feature map. 

 Input Image X Feature Detector = Feature Map. 

 the purpose of the feature detector is to detect a feature which is integral. The feature detecter has pattern in it . Even humans we also look at eveyone using a features and thats what feature maps gives us using feature detector.

 We create multiple feature map because we use different filters. We dont have just one feature map. The network decides which feature is important for certain types or certain categories.  

 ReLU
 -----
 We have input layer, We have the featuer maps, Now we are going to add the Rectifier. to increase Non Linearity in our network. because Images are highly non-linear. When you are applying convolution. We risk that we might create something linear so we need to break the linearilty. 

 ToDO : Check why do we need to break linearity using ReLU. Why a non-linear activation function in the essential output of all intermediatory layers. 

 Max Pooling
 -----------

 What is pooling and why do we need it. 
 - How can we detect one particilar image then how can our CNN find out about it ? 
 - We take the feature map. and take a 2x2 and run it through the feature map and collect the maximum number of the Feature map. 
 - If the photo is rotated we will still be able to preserve the feature and we'll be able to presenrve the feature. 
 - We are reducing 75% the number of parameters and hence we are preventing overfitting. 
 - By removing a non important function we are removing overfitting. 

 There is Mean Pooling , Average pooling

 Flattening
 -----------

 From the above steps we get a Pooled Feature Map. 

 After Flattening  -

 We put all the values in one column , We are going to flatten the into a column. We will later put this as a input in a Neural Network. Which will be out long vector which will be our Neural Network. 

 Full Connection. 
 ----------------

 Finally Adding the whole neural network to our convolutional neural network. WOW. 

 In CNN Hidden Layers have to be Fully Connected Layer and then this will be given to Output layer. 

 When we are doing a Classification we will have more than one output. 


 Network optimizes using BackPropagation. - from start to end the whole thing happens .. and then errors are found, Weights are distributed and finally 

 the signals are sent to both the classifiers .. in one example Dog and Cat. The Dog and Cat will know when a neuron are fired up. The more the CAT neuron are 
 
 These features are finally features which are sent to the network and they classify the network. 

 EPOCH is when you go throug the whole dataset once. 
 Something in the feature of Dogs and Cats. 

So eventually the Dog neuron and Cat neuron listens to various neurons 

Neurons which are present in the final layer get to vote. 
and the weights are importance that they get to the neurons. 


Summary
-------

Start with Input Image. 
Apply multiple feature detectors also called filters.
Crate Feature Maps. Which comprise of Convolutional Layer. 
On top of that apply ReLU to removing Linearity.
Apply Pooling. Pooling is done to make sure that it still keeps the data integreity , prevents overfitting and reduces size. Preserves main features. 

Then we flatten all the pooled images into a Single Dimensional Vector.
Then we finally have a layer. 
Very well defined network. 
Now this is passed on to Best feature maps. which can recognize 

