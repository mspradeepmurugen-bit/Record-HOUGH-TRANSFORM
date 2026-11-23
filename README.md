#  Lane Detection

##  Aim

To implement a basic lane detection pipeline using OpenCV by completing missing code segments at specified locations.

---

## Learning Objective

* Understand each stage of image processing
* Learn how to build a complete computer vision pipeline
* Practice writing code in guided sections

**Important Instruction:**
👉 Write code **ONLY in places marked as `# Your Code Here`**
👉 Do NOT modify any other part of the code

---

##  Software Used

* Anaconda – Python 3.7
* Jupyter Notebook / VS Code
* OpenCV (cv2)
* NumPy
* Matplotlib

---

##  Algorithm & Explanation

---

###  Step 1: Import Libraries

```python
import cv2
import numpy as np
import matplotlib.pyplot as plt
```
import cv2
import numpy as np
import matplotlib.pyplot as plt
---

###  Step 2: Read the Image

```python
# Read the image using OpenCV

###
image = cv2.imread('C:/Users/acer/Downloads/Qno. 1.jpg.jpeg')  # Replace 'image.jpg' with your image path
gray_image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
###
```

---

###  Step 3: Convert to Grayscale

```python
# Convert to grayscale.

###
Input image and grayscale image
plt.imshow(cv2.cvtColor(image, cv2.COLOR_BGR2RGB))  # Convert image to RGB for displaying
plt.title("Input Image")
plt.axis('off')
###
```

---

###  Step 4: Display Images

```python
plt.figure(figsize=(10,5))

###
plt.imshow(gray_image, cmap='gray')
plt.title("Grayscale Image")
plt.axis('off')
###
```

---

###  Step 5: Thresholding

```python
# Apply thresholding

threshold = 
###
plt.imshow(gray_image, cmap='gray')
# Canny Edge Detector output
plt.imshow(edges, cmap='gray')
plt.title("Canny Edge Detector")
plt.axis('off')
###
```

---

###  Step 6: Region of Interest (ROI)

```python
# ROI masking already provided
# (Do not modify)
```

---

### Step 7: Edge Detection (Canny)

```python
# Perform Edge Detection

###
# Step 5: Using the HoughLinesP(), detect line coordinates for every point in the image
# The parameters of HoughLinesP are: image, resolution, threshold, minLineLength, maxLineGap
lines = cv2.HoughLinesP(edges, 1, np.pi / 180, 100, minLineLength=50, maxLineGap=10)
###
```

---

###  Step 8: Gaussian Blur

```python
# Apply Gaussian Blur

###
# Step 5: Using the HoughLinesP(), detect line coordinates for every point in the image
# The parameters of HoughLinesP are: image, resolution, threshold, minLineLength, maxLineGap
lines = cv2.HoughLinesP(edges, 1, np.pi / 180, 100, minLineLength=50, maxLineGap=10)

###
```

---

###  Step 9: Hough Transform

```python
# Detect lines using Hough Transform

###
# Display the result of Hough Transform (Image with lines)
plt.imshow(cv2.cvtColor(image, cv2.COLOR_BGR2RGB))  # Image with lines drawn
plt.title("Result of Hough Transform")
plt.axis('off')
###
```

---

### Step 10: Lane Detection Logic

```python
# Already implemented
# (Do not modify)
```

---

##  Expected Output

* Original image
* Grayscale image
* Thresholded image
* ROI masked image
* Edge detected image
* Smoothed image
* Detected lines
* Final lane detection output

---

##  Instructions

* Fill ONLY in `# Your Code Here` sections
* Do NOT change existing code
* Run step-by-step
* Verify outputs

---

## Result

Thus, the lane detection pipeline is successfully implemented by completing the missing code sections. The system detects and highlights lane lines effectively.

---
## Output
<img width="472" height="495" alt="Screenshot 2026-11-23 145900" src="https://github.com/user-attachments/assets/4bec1262-985f-4320-90f4-1fd7fe6432e0" />
<img width="452" height="497" alt="Screenshot 2026-11-23 145907" src="https://github.com/user-attachments/assets/9edf00e9-55ce-4acd-93bd-0d73031e55e5" />
<img width="480" height="500" alt="Screenshot 2026-11-23 145912" src="https://github.com/user-attachments/assets/d8bd1086-4ac8-4748-bf53-f148bc546f85" />
<img width="462" height="507" alt="Screenshot 2026-11-23 145933" src="https://github.com/user-attachments/assets/a313ebd1-11ea-4a94-9323-fb826ec85dff" />


##  Developed By

* **Name:** Pradeep.M
* **Register No:** 212225220071 # Record-HOUGH-TRANSFORM
