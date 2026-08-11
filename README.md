# Nuclei-segmentation-scikit-image
#### Classical nuclei segmentation and evaluation of microscopy images using scikit-image. 

The pipeline uses scikit-image as the primary library for segmentation. Hardcoded values from histogram analysis are used for image cleaning and segmentation, and are adjusted specifically for BBBC039 U2OS nuclei segmentations. The pipeline is only made for that datase
60 different images out of 200 in the BBBC039 dataset were randomly selected to evaluate pipeline consistency and segmentation metrics. These metrics include, Intersection Over Union, Dice Similarity Coefficient, Hausdorff distance and Panoptic Quality(PQ). 

#### Libraries: 
- Python          : 3.12.13
- Pathlib         : Built-in (Standard Library)
- scikit-image    : 0.26.0
- stardist        : 0.9.2
- miseval         : 1.3.0
- numpy           : 2.4.6
- scipy           : 1.17.1
- matplotlib      : 3.11.0
- pandas          : 3.0.5

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


 ## Limitations: 
 This pipeline was run on an intel i5 CORE CPU, which limited large scale image processing through the CPU-run scikit-image pipeline. 
 Thus 60 different randomly selected images were used in evaluation. 
 - Due to the limitations of classical segmentation pipeline, hardcoded morphological values found through  histogram analysis were used for optimum segmentation quality
 - This segmentation pipeline can run well only on 2- dimensional images with somewhat defined objects with some intensity contrast from the background 
 






