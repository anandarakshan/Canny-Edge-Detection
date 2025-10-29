# Canny-Edge-Detection
## Name:Ananda Rakshan K V
## Reg.No: 212223230014
# AIM:
To implement Canny edge detection algorithm.

# Program:

```
import cv2
import matplotlib.pyplot as plt
# Read the image
img = cv2.imread('k.jpg',cv2.IMREAD_GRAYSCALE)
# Apply Gaussian blur to reduce noise
blurred =cv2.GaussianBlur(img, (5,5),0)
# Detect edges using Canny
edges = cv2.Canny(blurred, 50, 150) #Adjust threshold values as needed
# Plot the original image and the detected edges
plt.figure(figsize=(10,5))
plt.subplot(121),plt.imshow(img, cmap='gray')
plt.title('Original Image'), plt.axis('off')
plt.subplot(122),plt.imshow(edges, cmap='gray')
plt.title('Detected Edges'), plt.axis('off')
plt.show()
```

# Output:

<img width="964" height="530" alt="image" src="https://github.com/user-attachments/assets/03704783-813b-4adc-9ef9-f6e3f7ec7921" />

# Result:
Thus the Canny edge detection algorithm is implemented.
