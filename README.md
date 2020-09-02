# Hand-written-digit-classifier

-> The MNIST dataset is an acronym that stands for the Modified National Institute of Standards and Technology dataset.
(for more info visit their link:- http://yann.lecun.com/exdb/mnist/ )

-> It is a dataset of 60,000 small square 28×28 pixel grayscale images of hand written single digits between 0 and 9.

-> The task is to classify a given image of a handwritten digit into one of 10 classes representing integer values from 0 to 9, inclusively.


The code is written in python language with necessary libraries and comments are there for every step to understand it better. 

Result:-

  Output for 5 time runing code for full data set.
  
    Epoch 1/5
    1875/1875 [==============================] - 33s 18ms/step - loss: 0.4723 - accuracy: 0.8328
    Epoch 2/5
    1875/1875 [==============================] - 33s 18ms/step - loss: 0.3178 - accuracy: 0.8871
    Epoch 3/5
    1875/1875 [==============================] - 33s 18ms/step - loss: 0.2767 - accuracy: 0.8997
    Epoch 4/5
    1875/1875 [==============================] - 33s 18ms/step - loss: 0.2503 - accuracy: 0.9089
    Epoch 5/5
    1875/1875 [==============================] - 33s 18ms/step - loss: 0.2314 - accuracy: 0.9155
  
  predictoin and actual values for checking, is the model correct ?
 
    predicted:	 [9 2 1 1 6 1 4 6 5 7 4 5 8 3 4 1 2 4 8 0 2 5 7 5 1 6 6 0 9 3]
    Actual :	 [9 2 1 1 6 1 4 6 5 7 4 5 7 3 4 1 2 4 8 0 2 5 7 9 1 4 6 0 9 3]
    
  Here, 100 % accurate for 30 digit-images out of 60,000 test images.
  Let's proceed on full testing data.....

  
  Precision Matrix results are here that is created by using Convolutional Neural Networks (CNN) with sequential model adding relu and softmax activation function and adam optimizer to fit data.
  
    for digits: 0   1   2   3   4   5   6   7   8   9
    TP: [835 984 852 951 862 981 703 971 989 960]    (True positive)
    TN: [8895 8990 8848 8858 8832 8983 8786 8957 8969 8970]  (True Negative)
    FP: [105  10 152 142 168  17 214  43  31  30]    (False Positive)
    FN: [165  16 148  49 138  19 297  29  11  40]    (False Negative)
    
   Finally, results are...
    	  
        precision specificity F1_scores 	accuracy 	recall or sensitivity
    0 	0.888298 	0.988333  	0.860825  	0.9730 	    0.835
    1 	0.989940 	0.998889  	0.986961 	  0.9974    	0.984
    2 	0.848606 	0.983111  	0.850299  	0.9700 	    0.852
    3 	0.870082 	0.984222   	0.908743  	0.9809 	    0.951
    4 	0.836893 	0.981333 	  0.849261  	0.9694 	    0.862
    5 	0.982966 	0.998111  	0.981982  	0.9964 	    0.981
    6 	0.766630 	0.976222  	0.733438  	0.9489 	    0.703
    7 	0.957594 	0.995222  	0.964250  	0.9928 	    0.971
    8 	0.969608 	0.996556  	0.979208   	0.9958 	    0.989
    9 	0.969697 	0.996667  	0.964824  	0.9930 	    0.960
    
   Thanks for your patience to understaning clearly. 
