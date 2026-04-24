# Face Sunglasses Overlay

This project demonstrates how to programmatically overlay a pair of sunglasses onto a face image using Python and OpenCV. It explores image manipulation techniques, including resizing, alpha channel masking, and bitwise arithmetic to achieve a realistic blend.

## Project Overview

The notebook guides you through the process of:
1. **Loading Images**: Reading the base face image (`pic.jpeg`) and the sunglass image with an alpha channel (`sunglass.png`).
2. **Preprocessing**: Resizing the sunglasses to fit specific eye coordinates.
3. **Masking**: Extracting the alpha channel from the sunglass image to create a binary mask.
4. **Image Arithmetic**: 
   - Using the mask to "cut out" the eye region from the face.
   - Using the mask to extract only the visible parts of the sunglasses.
   - Combining both using `cv2.add` to create the final augmented image.

## Getting Started

### Prerequisites

You will need the following Python libraries installed:
- `opencv-python`
- `numpy`
- `matplotlib`

You can install them via pip:
```bash
pip install opencv-python numpy matplotlib