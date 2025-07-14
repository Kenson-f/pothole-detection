# Pothole Detection Using Image-Based Data Mining

A comprehensive image processing pipeline developed to detect potholes in road images without using pre-trained models. This project was built as part of a 2nd-year AI & DS course at Shiv Nadar University, Chennai.

---

## Features

- Manual grayscale conversion, Gaussian blur, adaptive thresholding
- Morphological operations (open, close) to clean binary images
- Contour detection & filtering based on:
  - Area
  - Perimeter
  - Circularity
  - Aspect ratio
  - Extent
  - Texture variation
- Edge analysis using Canny edge detection
- Composite scoring system for pothole confidence
- Visual output with pothole contours and scores

---

## Why Manual Implementation?

- Educational value: Understand how each algorithm works internally
- Avoid dependency on OpenCV for core functions
- Transparent, interpretable workflow
- Allows fine-tuning of parameters at each step

---

## Architecture

1. Convert to grayscale
2. Apply Gaussian blur
3. Adaptive thresholding
4. Morphological operations
5. Contour detection
6. Filter based on shape metrics
7. Texture & edge analysis
8. Composite scoring (0-1 scale)
9. Highlight potholes on output image

---

## Dataset Structure
1. Images with Pothole
2. Images with no Pothole


---

##  How to Run

###  Requirements
- Python 3.x
- `numpy`
- `matplotlib`
- `PIL` (Pillow)

### ▶️ Run Single Image Detection

```bash
python detect_potholes.py --image path/to/image.jpg --debug


