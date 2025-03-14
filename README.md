# Lane Detection using OpenCV

This project detects lane lines in road images using Python and OpenCV. The algorithm identifies lane boundaries to assist autonomous vehicles in navigation.

## Table of Contents

- [Overview](#overview)
- [Installation](#installation)
- [Pipeline Steps](#pipeline-steps)
- [Results](#results)
- [Challenges and Improvements](#challenges-and-improvements)
- [How to Run](#how-to-run)
- [Contributing](#contributing)
- [License](#license)
- [Colab Notebook](#colab-notebook)

## Overview

Lane detection is crucial for autonomous vehicles to understand road boundaries and safely navigate. This project implements a computer vision pipeline that processes images to detect lane lines.

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/mmanikandan281/Lane-Line-detection.git
   ```
2. Create a virtual environment (optional but recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use: venv\Scripts\activate
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Pipeline Steps

1. **Grayscale Conversion:** Convert the image to grayscale to simplify processing.
2. **Gaussian Blur:** Apply Gaussian blur to reduce noise.
3. **Edge Detection:** Use the Canny edge detection algorithm.
4. **Region of Interest (ROI):** Mask the image to focus on the lane area.
5. **Hough Transform:** Detect lines in the ROI.
6. **Line Extrapolation:** Average and extend detected lines to represent lanes.

## Results

The pipeline successfully detects lane lines in various road conditions. Below is an example of the output:



## Challenges and Improvements

- **Shadows and Lighting Conditions:** Performance drops under poor lighting.
- **Curved Lanes:** Current implementation works best on straight lanes.
- **Improvements:** Future enhancements could include advanced techniques like polynomial fitting for curved lanes or incorporating deep learning models.

## How to Run

1. Activate the virtual environment (if used):
   ```bash
   source venv/bin/activate
   ```
2. Run the Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
3. Open `P1.ipynb` and run each cell to see the lane detection pipeline in action.

## Contributing

Contributions are welcome! Feel free to fork the repo, create a branch, and submit a pull request.

## License

This project is licensed under the MIT License.

## Colab Notebook

You can also run the project on Google Colab using this [link](https://colab.research.google.com/drive/1ZHE1WAEOQChv1IT9Iy4ZxYXrVYWSu13L?usp=sharing).

---

Made with ❤️ by Manikandan M

