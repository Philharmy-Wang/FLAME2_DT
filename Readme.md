# FLAME2-DT Dataset (FLAME2 Dataset for Detection Tasks)

## 1. Introduction

FLAME2-DT is an enhanced version of the FLAME2 dataset, specifically optimized for multi-modal forest fire detection tasks. Built upon the original FLAME2 dataset's RGB-IR video pairs of prescribed burns, we have substantially improved its utility for object detection research through comprehensive pixel-level annotations and systematic data processing.

## 2. Dataset Development Process

1. **Data Collection and Processing**
   * Source: Selected high-quality video sequences from FLAME2 dataset
   * Spatial Registration: Applied feature point matching and transformation consistency analysis
   * Frame Extraction: Utilized adaptive frame-difference sampling strategy
   * Resolution: Maintained high-quality 640×512 resolution for both RGB and IR modalities
2. **Annotation Methodology**
   * Multi-expert cross-validation annotation protocol
   * Pixel-level precise bounding box labeling
   * Separate annotation for flame and smoke regions
   * Quality assurance through multi-round verification

## 3. Dataset Statistics and Characteristics

1. **Dataset Scale**

   * Total Image Pairs: 1,280
   * Training Set: 1,024 pairs (80%)
   * Validation Set: 256 pairs (20%)
2. **Annotation Statistics**
   RGB Images:

   * Flame Boxes: 2,496
   * Smoke Boxes: 4,404
   * Combined Annotations: 6,900

   IR Images:

   * Flame Boxes: 27,117
   * Smoke Boxes: Not applicable (thermal imaging cannot capture smoke)
3. **Target Characteristics Analysis**
   Flame Features:

   * Scale Distribution: Approximately 80% of flame bounding boxes occupy less than 5% of image area
   * Spatial Pattern: Multi-centered distribution with varying intensity levels
   * Temperature Signature: Clear thermal signatures in IR images

   Smoke Features:

   * Scale Distribution: Over 60% of smoke bounding boxes occupy more than 12% of image area
   * Visual Characteristics: Variable opacity and texture patterns
   * Visibility: Only detectable in RGB images

## 4. Dataset Organization

The dataset is structured into five specialized packages:

`origin_dataset.zip`

* Complete frame-extracted original images
* Full annotation files
* Raw data preservation

`RGB+RGB_labels.zip`

* RGB modality images
* Corresponding RGB-specific annotations
* Training/validation split

`IR+IR_labels.zip`

* Thermal infrared images
* IR-specific annotations
* Training/validation split

`RGB+RGB_IR_labels.zip`

* RGB images
* Combined RGB-IR annotations
* Optimized for multi-modal analysis

`RGB_IR_fuse_labels.zip`

* Complete RGB-IR image pairs
* Comprehensive annotation set
* Full multi-modal capability
* 

## 5. Applications

1. **Research Areas**

* Multi-modal object detection
* Forest fire monitoring
* Environmental protection
* Emergency response systems


**2. Algorithm Development**

* Deep learning model training
* Multi-modal fusion techniques
* Real-time detection systems

## 6. Citation and Usage

When using FLAME2-DT dataset in your research, please cite:

{......}
