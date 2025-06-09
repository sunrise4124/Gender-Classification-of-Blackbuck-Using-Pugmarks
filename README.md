# Gender-Classification-of-Blackbuck-Using-Pugmarks

This repository focuses on various techniques for extracting Regions of Interest (ROI) from images and proposes a Convolutional Neural Network (CNN) model for subsequent image analysis. The ROI extraction methods include both traditional image processing techniques and a naive approach based on saturation and brightness differences.

#

# Highlights:
Diverse ROI Extraction Techniques: Implements several methods for identifying regions of interest in images, including:

Naive Technique: Calculates the difference between saturation and brightness channels in HSV color space, applies thresholding, and selects the largest contour as the ROI.

Template Matching: Uses cv2.matchTemplate to find the ROI based on a predefined template.

Contour Detection: Identifies contours after thresholding a grayscale image and extracts the bounding box of the largest contour as the ROI.

Masking: Extracts ROI based on predefined mask ratios.

Edge Detection: Utilizes Canny edge detection to create a mask and apply it to the original image to highlight edge-based ROIs.

Combined Approach: Integrates the naive approach (saturation and brightness difference), contour detection, and masking for robust ROI extraction.

CNN Model for Image Analysis: Proposes a sequential CNN model designed to process images (presumably the extracted ROIs) for further tasks.

#

# Requirements:

The code snippets utilize common Python libraries for image processing and deep learning. You will need to install:

numpy

opencv-python (cv2)

Pillow (PIL, Image)

tensorflow (specifically tensorflow.keras)

#

# Dataset:

The sample data is provided in the Sample Dataset folder. The full dataset can be provided on request.

#

# Results:

Accuracy using Edge Detection: 96.38%

Accuracy using Contour Detection: 91.17%

Accuracy using Masking: 82.67%

Accuracy using Naive approach: 96.25%

#

# Citation:

If you are using the above code, then please cite this manuscript:
Dawar, A., Garg, D., Kakkar, P., Ragothaman, H., Bhardwaj, A., Rana, PS. (2025). Enhanced Gender Classification of Blackbucks via a Novel Convolutional Neural Network Using Pugmark Analysis, The Visual Computer, Springer.

#

# DOI Badge

10.5281/zenodo.15625673
