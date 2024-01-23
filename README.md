# OCR Text Extraction from Image

## Overview
This Python script utilizes the `easyocr` library along with `OpenCV` to perform Optical Character Recognition (OCR) on an image. The script reads text from the specified image file and displays the original image alongside the extracted text.

## How to Use
1. Ensure you have the required libraries installed (`easyocr`, `cv2`, `matplotlib`, and `numpy`).
2. Replace `IMAGE_PATH` with the path to your image file.
3. Run the script in a Python environment.

## Requirements
- Python 3.x
- `easyocr`
- `opencv-python` (cv2)
- `matplotlib`
- `numpy`

## Example
```python
IMAGE_PATH = 'surf.png'
reader = easyocr.Reader(['en'], gpu=False)
result = reader.readtext(IMAGE_PATH)
print(result)
