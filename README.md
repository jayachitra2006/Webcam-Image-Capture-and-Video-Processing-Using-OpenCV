# Image Capture and Video Processing Using OpenCV

---

## Aim

To write a Python program using OpenCV to capture an image from the webcam and perform the following operations:

1. Write the frame as a JPG file  
2. Display the video  
3. Display the video by resizing the window  
4. Rotate and display the video  

---

## 🛠️ Software Used

- Anaconda – Python 3.7  
- Jupyter Notebook / VS Code  
- OpenCV (`cv2`)  

---

## ⚙️ Algorithm

### Step 1:
Import the required libraries and initialize the webcam using `cv2.VideoCapture()`.

### Step 2:
Capture frames continuously from the webcam.

### Step 3:
Save a frame as a JPG image using `cv2.imwrite()`.

### Step 4:
Display the live video stream using `cv2.imshow()`.

### Step 5:
Resize the frame and rotate it using OpenCV functions, then display the processed frames.

---

## 💻 Program
import cv2

captured_image = cv2.imread("WIN_20260728_11_06_56_Pro.jpg")

if captured_image is None:
    print("Image not found!")
else:
    print("Image loaded successfully.")
 ## Then display it
 import matplotlib.pyplot as plt

plt.imshow(cv2.cvtColor(captured_image, cv2.COLOR_BGR2RGB))
plt.title("Original Image")
plt.axis("off")
plt.show()
## Resize it
resized_image = cv2.resize(captured_image, (100, 150))

plt.imshow(cv2.cvtColor(resized_image, cv2.COLOR_BGR2RGB))
plt.title("Resized Image")
plt.axis("off")
plt.show()
## Rotate it
rotated_image = cv2.rotate(captured_image, cv2.ROTATE_90_CLOCKWISE)

plt.imshow(cv2.cvtColor(rotated_image, cv2.COLOR_BGR2RGB))
plt.title("Rotated Image")
plt.axis("off")
plt.show()

### Developed By:
**Name:** jayachitra j

### Register No:
212224040132

---

## Output

### i) Write the frame as JPG image
Captured image is saved as <img width="515" height="319" alt="download" src="https://github.com/user-attachments/assets/448fd6a5-4ba4-4f8e-9580-93467adcc97d" />


### ii) Display the video
Live webcam video is displayed
<img width="1280" height="720" alt="WIN_20260728_11_06_56_Pro" src="https://github.com/user-attachments/assets/87fc7314-9cbb-475d-93e7-0b925e45724f" />


### iii) Display the video by resizing the window

<img width="266" height="409" alt="download" src="https://github.com/user-attachments/assets/392d2ee1-8eff-41d2-a6d7-5bf90464be00" />

Video is shown in resized resolution (640 × 480)

### iv) Rotate and display the video
<img width="227" height="409" alt="download" src="https://github.com/user-attachments/assets/255c6406-aabb-4516-8f05-43d4f6574eca" />


Video is displayed after rotation (90° clockwise)

---

## Result

Thus, the image is successfully captured from the webcam and various video processing operations such as saving, displaying, resizing, and rotating are performed using OpenCV.
