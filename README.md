# Image Segmentation and Active Contour Using scikit-image

# Description
This project focuses on image segmentation techniques using Python's scikit-image library. The main goal is to segment objects from an image by applying various methods such as active contours (snakes), circle perimeters, random walker segmentation, and superpixel segmentation (SLIC). The project demonstrates how to extract a region of interest (ROI) and segment the desired object from an image, applying smooth curves around the edges and processing them for further analysis.

# Requirements
To run the project, install the following dependencies:

 ![image](https://github.com/user-attachments/assets/db0e5146-bac5-4d2d-b056-43d6164ea898)
![indexx](https://github.com/user-attachments/assets/45adbe53-66af-4505-9d07-02b7999df50d)

pip install numpy
pip install matplotlib
pip install scikit-image

# Project Workflow
- Load an Image: The project begins by importing an image using skimage.io.imread().

- Convert Image to Grayscale: The RGB image is converted to grayscale using skimage.color.rgb2gray() to simplify processing.

- Draw Circle on Image: The initial region of interest is drawn as a circle using polar coordinates.

- Active Contour (Snake Algorithm): The active contour method (seg.active_contour()) is applied to segment the object of interest (in this case, the sun).

- Circle Perimeter Labeling: The circle perimeter is drawn around a specific point in the image, and the segmented regions are labeled.

- Random Walker Segmentation: This method refines the segmentation using pre-labeled pixels as the seed points.

- Superpixel Segmentation (SLIC): The image is divided into superpixels using seg.slic(), which reduces the complexity of the image and provides average colors for each region.

Key Files
tp3 tim.py: Contains the code to load the image, perform segmentation, and visualize the results.
image.jpg: Input image for testing the segmentation algorithms.
