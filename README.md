# EC7212 - Computer Vision and Image Processing - Assignment 2

This repository contains the implementation of two computer vision techniques for **EC7212 - Computer Vision and Image Processing Take Home Assignment 2**.

## 📋 Assignment Overview

This assignment demonstrates the implementation of fundamental image processing algorithms:
1. **Otsu's Thresholding Algorithm** with Gaussian noise
2. **Region Growing Segmentation** technique

## 🗂️ Project Structure

```
Assignment 02 - 4276/
├── assignment2_4276.ipynb    # Main Jupyter notebook with implementations
├── task1.png                 # Input image for Task 1
├── task02.jpg               # Input image for Task 2
├── task01_output.png        # Output visualization for Task 1
├── task02_output.png        # Output visualization for Task 2
└── README.md               # This file
```

## 📝 Tasks Description

### Task 1: Otsu's Thresholding Algorithm

**Objective**: Implement and test Otsu's algorithm on an image with 2 objects and background (3 pixel values total) after adding Gaussian noise.

**Implementation Features**:
- Custom image creation with 3 distinct pixel values
- Gaussian noise addition function
- Complete Otsu's algorithm implementation from scratch
- Visualization of original image, noisy image, thresholded result, and histogram

**Key Functions**:
- `add_gaussian_noise()`: Adds Gaussian noise to input image
- `otsu()`: Implements Otsu's automatic thresholding algorithm

### Task 2: Region Growing Segmentation

**Objective**: Implement a region-growing technique for image segmentation starting from seed points and expanding based on pixel value similarity.

**Implementation Features**:
- Interactive seed point selection
- Recursive region growing algorithm
- Threshold-based pixel inclusion criteria
- Visualization of original image with seed points and segmentation result

**Key Functions**:
- `region_growing()`: Main segmentation algorithm that grows regions from seed points

## 🚀 Getting Started

### Prerequisites

Make sure you have the following libraries installed:

```python
import cv2
import numpy as np
import matplotlib.pyplot as plt
```

### Installation

1. Clone or download this repository
2. Install required dependencies:
   ```bash
   pip install opencv-python numpy matplotlib
   ```

### Running the Code

1. Open the Jupyter notebook:
   ```bash
   jupyter notebook assignment2_4276.ipynb
   ```

2. Run all cells sequentially to execute both tasks

3. The output images will be automatically saved as:
   - `task01_output.png` - Otsu's thresholding results
   - `task02_output.png` - Region growing segmentation results

## 🔧 Algorithm Details

### Otsu's Thresholding
- Automatically determines optimal threshold value
- Maximizes between-class variance
- Effective for bimodal histograms
- Robust against noise when properly implemented

### Region Growing
- Uses seed points as starting locations
- Expands regions based on pixel intensity similarity
- Configurable threshold parameter for growth control
- 8-connectivity neighborhood exploration

## 📊 Results

The implementations successfully demonstrate:

1. **Task 1**: Clean separation of objects from background despite Gaussian noise
2. **Task 2**: Accurate segmentation of regions of interest using seed-based growing

Output visualizations include:
- Original and processed images side-by-side
- Histogram analysis with threshold visualization
- Segmentation masks and overlays


---

*This implementation serves as a comprehensive demonstration of fundamental computer vision techniques for educational purposes.*
