# nuclei-segmentation-scikit-image
Classical nuclei segmentation and evaluation of microscopy images using scikit-image. 

The pipeline uses python, scikit-image, SciPy and NumPy to identify nuclei and separate clustered nuclei without deep learning. 
60 different images out of 200 in the BBBC039 dataset were randomly selected to evaluate pipeline consistency and segmentation metrics. These metrics include, Intersection Over Union, Dice Similarity Coefficient, Hausdorff distance and Panoptic Quality(PQ)
