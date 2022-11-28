
## REVERSE VISUAL SEARCH

The following requirements are to be done on the MS COCO dataset images and specifically for images of CLASS PERSON from the dataset provided.

## 1. LOADING THE DATASETOF CLASS PERSON
Your images will be from the MSCOCO mini dataset and will be of class person. 

## 2. PERFORMING OBJECT DETECTION ON A PRETRAINED MODEL
Using a model pretrained to perform object detection on MS COCO (e.g. https://pytorch.org/vision/stable/models/faster_rcnn.html ) extract the bounding boxes of all people in your dataset. 

## 3. REVERSE IMAGE SEARCH - FEATURE EXTRACTION
AWS is suggesting to build a reverse image search system.
Using eg. ResNet-50 as a featurizer (ensure that is the featurizer used by the object detector), extract for each detected bounding box the representation vector (2048 elements long).

## 4. REVERSE IMAGE SEARCH - SIMILARITY SEARCH
Using five (5) of the person bounding boxes as query, pick a similarity search python library to return the 10 most similar bounded boxed persons to the query image.Before you can execute the similarity search, you may have to do dimensionality reduction - clearly explain how you did that.
Select carefully the query image so that the results can be revealing of the ability of your representation and the search engine.

