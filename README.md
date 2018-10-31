# DIET dataset
Depth Intricate Estimation for Trees dataset
Early Experience of Depth Estimation on Intricate Objects 
Using Generative Adversarial Networks

The complexity of an object which can be attributed to its unpredictable structure and environmental lighting can make accurate depth estimation challenging. The human eye observes each part of an object with a different focus whereas computer vision defines a region of pixels to a focus that is likely to be incorrectly predicted in the context of complex objects.   In this work, we aim to exploit the effectiveness of conditional Generative Adversarial Networks (GAN) to improve depth estimation from a singular inexpensive monocular camera sensor.  We propose to use the light-field cameras to obtain good depth ground truth for outdoor complex objects. The Depth Intricate Estimation of Trees dataset (DIET) comprises of 128 photo-depth pairs of trees, which vary in structure and seasonal changes. 
  

Dataset Information
The apple trees are in the Yarra Valley (located in Melbourne, Victoria, Australia). The photos were taken in the Yarra Valley and processed at The University of Queensland (located in Brisbane, Queensland, Australia).  
Current Description (October 2018):
•	64 different tree photos taken in Spring and another 64 depth images to match these.
•	64 different tree photos taken in Summer and another 64 depth images to match these.
•	Photos are taken during the day with uncontrolled lighting (unpredictable weather). 
•	Each image is of 1404 x 2022 pixels for both RGB photo and depth image.
•	The photo and depth images are aligned. 
•	The image name for the photo and depth pair have the same number.
Evaluation Protocol: 
We utilise the evaluation metrics of Mean Square Error (MSE), Relative Error (REL), Structural Similarity (SSIM) and Signal-to-noise Ratio (PSNR)  on patches outputted by a generative adversarial network (GAN) of similar structure to Pix2Pix (Isola et al.). This was done by splitting up the images in the DIET dataset into patches of size 256 x 256 to be improve optimality of training time. A CSV file containing the directory address of the image patch and its name was used for training the GAN. This can be modified by the user who downloads the dataset because the CSV file is unique to the user.  
Training:  If have train.py can use a .csv file of the location paths for the training patches and photo pairs. A checkpoint should be saved once the train.py is finished to save the model.
Testing: Can load the checkpoint from the training step and restore the model and input the .csv file containing the test image photo patches to do the depth map conversion.
License
The DIET dataset (‘Licensed Material’) are made available to the non-commerical and scientific communities for academic, teaching and scientific purposes. Permission is granted to you (‘the Licensee’) to use the dataset with these conditions. Please include a reference to the following published work:

Wai Y. K. San, Teng Zhang, Shaokang Chen, Arnold Wiliem, Dario Stefanelli, Brian C. Lovell. “Early Experience of Depth Estimation on Intricate Objects Using Generative Adversarial Networks.” Digital Imaging and Computing Techniques Australia (DICTA), 2018.

Download
The current version of the DIET dataset can be downloaded here [download].
Citation
Wai Y. K. San, Teng Zhang, Shaokang Chen, Arnold Wiliem, Dario Stefanelli, Brian C. Lovell. “Early Experience of Depth Estimation on Intricate Objects Using Generative Adversarial Networks.” Digital Imaging and Computing Techniques Australia (DICTA), 2018. [pdf]
