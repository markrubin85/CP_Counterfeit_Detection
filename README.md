# Image Classification for Real & Counterfeit Colombian Peso Banknotes

# Business Problem:
Colombia has been fighting a massive  issue of people printing and using counterfeit currency. With the large amount of counterfeit currency that is currently in circulation and the widespread use of smartphones,  there is a widespread need for an application that uses a Deep Learning Algorithm to accurately determine the authenticity of Colombian Pesos in real-time.

# Scholarly Article Reference:
Title: Fake Banknote Recognition Using Deep Learning
 ## Url:
  https://www.mdpi.com/2076-3417/11/3/1281 
 ## Citation:
  Pachón, C.G.; Ballesteros, D.M.; Renza, D. Fake Banknote Recognition Using Deep Learning. Appl. Sci. 2021, 11, 1281. https://doi.org/10.3390/app11031281

# Data Source Reference:
Dataset was sourced from Mendeley Data
  ## Url:
  https://data.mendeley.com/datasets/tj8kvrbfz6/2 
  ## Citation:
  Pachon Suescun, Cesar; Ballesteros, Dora Maria; Renza, Diego (2021), “Original and counterfeit Colombian peso banknotes”, Mendeley Data, V2, doi: 10.17632/tj8kvrbfz6.2

# Data:
-Organized into 3 Folders each containing the same 7,280 images  but split using different locations for the Train, Test, and Validation Sets.
-Folders Included:
  -7,280 Images
  -Training Dataset - 4,368 Images
  -Testing & Validation Datasets - 1,456 Images Each
-Data included Rotational and Partial views of the banknotes.
-The banknote images were captured under UV light.

-Data Contains 13 Classes:
  -6 Classes of Authentic Banknotes
    -2k, 5k, 10k, 20k, 50k, 100k Denominations
  -6 Classes of Counterfeit Banknotes
    -2kf, 5kf, 10kf, 20kf, 50kf, 100kf Denominations 
  -1 Background Class
    -When there is no banknote in the captured image.
-All Classes are balanced in the number of images. 
  -560 Images per class.

# Modeling:
-Transfer Learning Modeling:
  -ResNet50
  -InceptionV3
  -AlexNet
-Custom Modeling (As described in the Scholary Article Cited Above):
  -Sequential Architecture:
    -Input Image is (224, 224, 3)
    -Followed by 5 Convolutional Layers (CL) & 3 Fully Connected (FC) Layers
      -All CL’s use Relu Activation
    -The last FC Layer has 13 outputs for the corresponding 13 classes.
      -Softmax Activation is implemented in the last FC Layer to obtain the probability of belonging to each class.
    -Lastly 2 Dropout layers were added to avoid overfitting.	


# Results:
Accuracy Metric Scores:
 -Custom Model:
    -Test: .9272
    -Validation: .9183
  
  -ResNet50
    -Test: .9973
    -Validation: 1.000

  -InceptionV3
    -Test: .8839
    -Validation: .8963

The ResNet50 model had the best results in terms of:
  -Accuracy 
  -Speed of convergence. 
Pixel Intensity: 
Images containing Fake/Counterfeit Currency had significantly larger mean pixel intensity values than the images containing Real denominations.



# Next Steps:
-Build a user friendly front end application.
-Source more data on Colombian Peso Banknotes.
-Source data for other currencies due to the issues surrounding counterfeit currency globally.


