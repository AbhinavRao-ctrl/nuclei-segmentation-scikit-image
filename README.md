# nuclei-segmentation-scikit-image
Classical nuclei segmentation and evaluation of microscopy images using scikit-image. 

The pipeline uses scikit-image as the primary library for segmentation. Hardcoded values from histogram analysis are used for image cleaning and segmentation, and are adjusted specifically for BBBC)39 U2OS nuclei segmentations. 
60 different images out of 200 in the BBBC039 dataset were randomly selected to evaluate pipeline consistency and segmentation metrics. These metrics include, Intersection Over Union, Dice Similarity Coefficient, Hausdorff distance and Panoptic Quality(PQ). 
#Examples
