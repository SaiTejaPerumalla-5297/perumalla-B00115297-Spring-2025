# perumalla-B00115297-Spring-2025
Dental Health Detection

Updates:
During data pre processing after executing the normalise images script, the expected result was creating a normalised images for test, train, valid folders with labels.
But I have encountered a problem where the labels were not created but the images were normalised. Henceforth I have made a new file named fix_labels.ipynb to create the labels for the images.

The next step is EDA. In this the first one is for checking the imbalance in the classes and found out that fillings class has much more images than the other classes. To handle this we have to the data augmentation.

In data augmentation step I encountered a new problem where the class folders were empty, I ran a new script to move the images by classes and re run the data augmentation file.

Next step is to re run class distribution script to check the imabalances.


Update this week: written a small script to check the verification of augmentaion and the augmentaion was succesful with the following cavity: 4718 images
 fillings: 490 images
 impacted tooth: 4957 images
 implant: 3848 images

 After re running class distribution script I found out that there were still imbalances with the data set distribution and then I had to make changes in the augmentation script and created a new file for augmentation and is success with all the categories having 5000 images.

 Replaced the class distribution file after re running with new augmented data.
