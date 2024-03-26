---

# Image Colorization using Deep Learning

This script is based on the work by Richard Zhang for image colorization using deep learning. The script colorizes grayscale images using pre-trained models and requires OpenCV and NumPy libraries.

## Installation

1. Make sure you have Python installed on your system. If not, download and install it from [python.org](https://www.python.org/downloads/).

2. Install the required libraries using pip:
   ```bash
   pip install numpy opencv-python
   ```

3. Download the pre-trained models from the following links:
   - [colorization_deploy_v2.prototxt](https://github.com/richzhang/colorization/blob/caffe/colorization/models/colorization_deploy_v2.prototxt)
   - [colorization_release_v2.caffemodel](https://github.com/richzhang/colorization/blob/caffe/colorization/models/colorization_release_v2.caffemodel)
   
4. Download `pts_in_hull.npy` from [here](https://github.com/richzhang/colorization/blob/caffe/colorization/resources/pts_in_hull.npy).

5. Place the downloaded files in the `models/` directory of this project.

## Usage

1. Update the paths in the script according to your system for the following variables:
   - `prototxt_path`: Path to the `colorization_deploy_v2.prototxt` file.
   - `model_path`: Path to the `colorization_release_v2.caffemodel` file.
   - `kernel_path`: Path to the `pts_in_hull.npy` file.
   - `image_path`: Path to the grayscale image you want to colorize.

2. Run the script using Python:
   ```bash
   python main.py
   ```

3. The colorized image will be displayed in a new window.

## Dependencies

- Python 3.x
- NumPy
- OpenCV

## Acknowledgments

- This project is based on the work by Richard Zhang and collaborators on image colorization using deep learning.

---
