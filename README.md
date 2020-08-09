# GRiD-R2-2020

This repo contains the code base used by us in order to complete the Flipkart Grid Challenge Round 2 on the Fashion problem.
It consists of 4 .ipynb notebooks, to be opened using colab, which are:

1. [DeepFashion_trained.ipynb](https://colab.research.google.com/github/ShivenTripathi/GRiD-R2-2020/blob/master/DeepFashion_trained.ipynb)  
It is the backbone of our model pipeline. In this, we are cloning the mmfashion model which has been pretrained already.
The mmfashion model has been developed by [open-mmlab](https://github.com/open-mmlab)
 
2. [dataset_creator.ipynb ](https://colab.research.google.com/drive/1GxfyGyVAuZykABbax3oWVoQVDV77ugrd?usp=sharing)  
This notebook creates the dataset used by us in our model. This notebook finds all the products belonging to a particular category on [nordstrom.com] (such as polo tshirts, tank tops, etc) and extracts the URL the images of those products, and stores them in a given directory, in the form of excel sheets.  
[Click here](https://drive.google.com/drive/folders/1ZQtOIMPMqhp-zUPfdXme-iU616UjMuZO?usp=sharing) to view our created dataset. 

3. [trends_from_attributes.ipynb](https://colab.research.google.com/drive/1ZIrM0MYO_sZBnWwER7iZb4a81AcRmewu?usp=sharing)  
This notebook utilizes the mmfashion model in order to make predictions on trendiness of  clothes and styles, by calculating the t-SNE embeddings of input images in any given range of time and then creating clusters of common styles together. This gives out the most trending fashion items in that given range of time, and also outputs then trends (attributes) which were the most popular and least popular in that period of timee.

4. [trends_from_attributes.ipynb](https://colab.research.google.com/drive/1tPWaVH2dGYInp04NTxrnePebIKWmUxpi?usp=sharing)
Another end product of our project: a Predictor for each attribute. This relies on an XGBoost based regressor and tells us future value of an attribute based on previous time steps’s values.

--------------------------------------------
Team Name: IITKianDoge
Team Members: 
1. Shiven Tripathi
2. Rishabh Dugaye
3. Atharv Singh Patlan
IIT Kanpur
