
# Video and Image Resizer using OpenCV

This repository contains a simple script that demonstrates how to resize videos and images using the OpenCV library in Python. Resizing allows you to adjust the dimensions of videos and images while maintaining their aspect ratios.

## Prerequisites

Make sure you have the following prerequisites installed:

- Python 3.x
- OpenCV library (`cv2`)

You can install the OpenCV library using the following command:

```bash
pip install opencv-python
```

## Usage

1. Clone this repository or download the script (`resize.py`).
2. Run the script using a Python interpreter.

```bash
python resize.py
```

3. The script captures video from your webcam (you can modify this to read from a video file) and displays both the original video and the resized video.

## How it works

The script defines a function called `resizer` that takes an image and a scale factor as input and returns the resized image using OpenCV's `cv2.resize` function. The `interpolation` parameter is set to `cv2.INTER_AREA` for better quality.

The main loop captures frames from the webcam, resizes them using the `resizer` function, and displays both the original and resized frames using OpenCV's `cv2.imshow`.

## Customization

- You can adjust the `scale` parameter in the `resizer` function to control the resizing factor.
- To resize images, replace the `cap` with the path to your image, and call the `resizer` function with the image.

```python
img = cv2.imread('path_to_image.jpg')
img_resize = resizer(img)
cv2.imshow("image", img)
cv2.imshow("image_sized", img_resize)
```

## Acknowledgements

This script is provided as a simple example of resizing videos and images using the OpenCV library.

---

Feel free to customize this README to match your repository's structure and style. You can add more details, examples, and explanations as needed.





