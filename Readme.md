# FLAME2-DT Dataset (Forest Fire Detection Dataset with Dual-modality Labels)

## Quick Links
* **Download**: 
  - Baidu Netdisk: https://pan.baidu.com/s/1bTm04RSyCaLC5TlmZG6SkQ?pwd=qfds 
  - Extraction Code: qfds

## 1. Introduction

FLAME2-DT is an enhanced version of the FLAME2 dataset, specifically designed for multi-modal forest fire detection research. The dataset features paired RGB-thermal infrared images captured by a Mavic 2 Enterprise Advanced UAV system, with comprehensive pixel-level annotations for both fire and smoke regions. This dataset aims to address the limitations in the original FLAME2 dataset, including missing annotations, resolution constraints, and spatial registration biases.



![fig_2_00](https://github.com/user-attachments/assets/b582b0b0-9b2b-4abe-9585-73ceb096515a)

*Fig. 1: Statistical analysis of multi-modal fire detection dataset.*

## 2. Dataset Characteristics

### Target Distribution Analysis

![fig_3_00](https://github.com/user-attachments/assets/f273cf27-2e3a-4ff5-b45f-d7aae4908ad9)

*Fig. 2: Analysis of size and spatial distribution characteristics. (a) Fire bounding box size distribution heat map; (b) Smoke bounding box size distribution heat map; (c) Fire bounding box center point distribution heat map; (d) Smoke bounding box center point distribution heat map. Colors from light to dark indicate distribution density from low to high.*

Key findings from statistical analysis:

1. **Scale Characteristics**
   * Fire: ~80% of bounding boxes occupy <5% of image area (small-scale, discrete distribution)
   * Smoke: >60% of bounding boxes occupy >12% of image area (large-scale, continuous distribution)

2. **Spatial Distribution**
   * Fire: Multi-centered, scattered pattern
   * Smoke: Relatively dispersed distribution of center points

## 3. Dataset Development

### Data Collection
* Equipment: Mavic 2 Enterprise Advanced UAV dual-camera system
* Resolution: 640×512 pixels (both RGB and thermal IR)
* Processing: Feature point matching and spatial transformation consistency analysis

### Annotation Protocol
* Multi-expert cross-validation strategy
* Pixel-level precise labeling
* RGB Images: 
  - 2,496 fire bounding boxes
  - 4,404 smoke bounding boxes
* Thermal IR Images:
  - 27,117 fire bounding boxes
  - No smoke annotations (due to thermal imaging limitations)

## 4. Dataset Organization

The dataset contains five specialized packages:

1. **origin_dataset**
   * Complete frame-extracted original images
   * Full annotation files

2. **RGB+RGB_labels**
   * RGB modality images
   * RGB-specific annotations
   * Training/validation split

3. **IR+IR_labels**
   * Thermal infrared images
   * IR-specific annotations
   * Training/validation split

4. **RGB+RGB_IR_labels**
   * RGB images
   * Combined RGB-IR annotations
   * Multi-modal analysis optimization

5. **RGB_IR_fuse_labels**
   * Complete RGB-IR image pairs
   * Comprehensive annotation set
   * Full multi-modal capability

## 5. Dataset Scale
* Total Image Pairs: 1,280
* Training Set: 1,024 pairs (80%)
* Validation Set: 256 pairs (20%)

## 6. Applications

### Primary Research Areas
* UAV-based forest fire detection
* Multi-modal object detection
* Remote sensing image analysis
* Emergency response systems

### Technical Development
* Multi-modal fusion algorithms
* Lightweight deep learning models
* Real-time detection systems

## 7. Citation

If you use the FLAME2-DT dataset in your research, please cite our paper:
......

