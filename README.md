# CP_Counterfeit_Detection
Colombia has been fighting a massive  issue of people printing and using counterfeit currency. With the large amount of counterfeit currency that is currently in circulation and the widespread use of smartphones,  there is a widespread need for an application that uses a Deep Learning Algorithm to accurately determine the authenticity of Colombian Pesos in real-time.

Dataset was sourced from Mendeley Data
  https://data.mendeley.com/datasets/tj8kvrbfz6/2 
  Pachon Suescun, Cesar; Ballesteros, Dora Maria; Renza, Diego (2021), “Original and counterfeit Colombian peso banknotes”, Mendeley Data, V2, doi: 10.17632/tj8kvrbfz6.2

Organized into 3 Folders each containing the same 7,280 images  but split using different locations for the Train, Test, and Validation Sets.
Folders Included:
  7,280 Images
  Training Dataset - 4,368 Images
  Testing & Validation Datasets - 1,456 Images Each
Data included Rotational and Partial views of the banknotes.
The banknote images were captured under UV light.

13 Classes:
6 Classes of Authentic Banknotes
2k, 5k, 10k, 20k, 50k, 100k Denominations
6 Classes of Counterfeit Banknotes
2kf, 5kf, 10kf, 20kf, 50kf, 100kf Denominations 
1 Background Class
When there is no banknote in the captured image.
All Classes are balanced in the number of images. 
560 Images per class.


Scholarly Article Sources:
https://www.mdpi.com/2076-3417/11/3/1281 
Pachón, C.G.; Ballesteros, D.M.; Renza, D. Fake Banknote Recognition Using Deep Learning. Appl. Sci. 2021, 11, 1281. https://doi.org/10.3390/app11031281
