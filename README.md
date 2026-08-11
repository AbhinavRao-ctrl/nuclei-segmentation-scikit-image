# Nuclei-segmentation-scikit-image
#### Classical nuclei segmentation and evaluation of microscopy images using scikit-image. 

The pipeline uses scikit-image as the primary library for segmentation. Hardcoded values from histogram analysis are used for image cleaning and segmentation, and are adjusted specifically for BBBC039 U2OS nuclei segmentations. The pipeline is only made for that datase
60 different images out of 200 in the BBBC039 dataset were randomly selected to evaluate pipeline consistency and segmentation metrics. These metrics include, Intersection Over Union, Dice Similarity Coefficient, Hausdorff distance and Panoptic Quality(PQ). 

## Segmentation Examples
The images have shuffled color-masks for easier cell boundary differentiation 

### 1: Fragmented nuclei 
<img width="6000" height="1800" alt="Segmentation_Example1" src="https://github.com/user-attachments/assets/8992ffdd-8727-4f41-b27b-c3cc1d52187a" />

### 2: Clustered Nuclei
<img width="12110" height="2233" alt="crowded_nuclei" src="https://github.com/user-attachments/assets/1685b319-9532-4565-874c-98fb295baf76" />

## Overlay comparison to original Image 
<img width="12117" height="2338" alt="overlay" src="https://github.com/user-attachments/assets/45464702-d72d-4164-b98c-a7c7337bf7ca" />


## Image pipeline progression: 
### Flowchart:
<img width="1677" height="2950" alt="Segmentation_pipeline_Flowchart" src="https://github.com/user-attachments/assets/850912b0-2b03-455f-8265-b7459e57af3a" />

### Original image through pipeline: 
<img width="11992" height="1997" alt="preprocessing" src="https://github.com/user-attachments/assets/8ba56b9a-89d4-4707-9b91-7b13c61d9197" />






