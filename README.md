# currency_note_authentication Authentication using OpenCV

This project uses **template matching** with OpenCV to verify whether a given currency note image is **genuine** or **fake**, based on a reference (authentic) image.

## 📌 Overview

The program compares a test image of a currency note against a reference image (genuine note) and determines its authenticity using `cv2.matchTemplate`. If the match confidence exceeds a set threshold, the note is classified as genuine.

## 🧪 How It Works

1. Loads a **reference image** of a known genuine note.
2. Loads the **test image** to be authenticated.
3. Resizes the test image to match the reference image.
4. Applies **template matching** using `cv2.TM_CCOEFF_NORMED`.
5. If the confidence is higher than a threshold (default: `0.8`), it declares the note **genuine**; otherwise, **fake**.
6. Displays the result with bounding box and status text.


## 🛠️ Requirements

- Python 3.x
- OpenCV
- NumPy

### Install dependencies

```bash
pip install opencv-python numpy
