# Computer Vision and Image Processing - Assignment 2

**Course:** EC7212 - Computer Vision and Image Processing  
**Assignment:** Take Home Assignment 2  
**Focus:** Image Segmentation Techniques

## Overview

This assignment implements two fundamental image processing operations for computer vision applications:

1. **Task 01:** Otsu's Automatic Thresholding with Gaussian Noise Handling
2. **Task 02:** Region Growing Segmentation Technique

Both tasks demonstrate practical approaches to image segmentation, which is crucial for object detection, image analysis, and computer vision applications.

## Project Structure

```
assignment-2/
├── README.md
├── task01.py                 # Otsu's thresholding implementation
├── task02.py                 # Region growing segmentation
├── task01_input.png          # Input image for Task 1
├── task02_input.jpg          # Input image for Task 2
├── task01_output.png         # Generated output for Task 1
├── task02_output.png         # Generated output for Task 2
└── requirements.txt          # Python dependencies
```


## Usage Instructions

### Running Task 01
```bash
python task01.py
```

**Prerequisites:**
- Place input image as `task01_input.png` in the same directory
- Ensure image contains objects with distinct intensity levels

**Output:**
- `task01_output.png`: Visualization showing original, noisy, binary, and histogram
- Console output with threshold value and statistics

### Running Task 02
```bash
python task02.py
```

**Prerequisites:**
- Place input image as `task02_input.jpg` in the same directory
- Modify seed points in code if needed: `seed_coordinates = [(x1,y1), (x2,y2), ...]`

**Output:**
- `task02_output.png`: Side-by-side comparison of original with seeds and segmentation result
- Console output with segmentation statistics


## Configuration Options

### Task 01 Parameters
```python
# Gaussian noise parameters
mean_val = 0        # Noise mean
std_dev = 20        # Noise standard deviation

# Otsu parameters are automatically calculated
```

### Task 02 Parameters
```python
# Seed points (modify as needed)
seed_coordinates = [(100, 150), (120, 170), (180, 170), (190, 150)]

# Intensity threshold
intensity_threshold = 10  # Adjust based on image characteristics
```

## Expected Results

### Task 01 Output
- **Original Image:** Color/grayscale input image
- **Noisy Image:** Grayscale with added Gaussian noise
- **Binary Segmentation:** Black and white segmented result
- **Histogram:** Intensity distribution with optimal threshold line

### Task 02 Output
- **Original with Seeds:** Input image with red circular markers at seed points
- **Segmentation Result:** Binary mask showing grown regions (white) vs background (black)

## Performance Metrics

### Task 01 Metrics
- Optimal threshold value
- Image dimensions 
- Pixel count

### Task 02 Metrics
- Number of seed points
- Segmentation percentage
- Seed coordinates
- Intensity threshold
- Segmented pixels
- Segmentation percentage






