import cv2
import numpy as np

# Initialize a global list to store circle centers
circles = []

# Mouse callback function
def draw_circle(event, x, y, flags, param):
    global circles
    if event == cv2.EVENT_LBUTTONDOWN:  # Check if left mouse button was clicked
        circles.append((x, y))  # Append the position of the click
        # Draw the circle on the image
        cv2.circle(image, (x, y), radius, color, thickness)
        # Display the updated image
        cv2.imshow('Drawing Circles', image)

# Create a black image
image = np.zeros((500, 500, 3), dtype=np.uint8)

# Set circle parameters
radius = 20
color = (0, 255, 0)  # Green color in BGR
thickness = 2

# Create a window and set the mouse callback function
cv2.namedWindow('Drawing Circles')
cv2.setMouseCallback('Drawing Circles', draw_circle)

print("Click on the window to draw circles. Press 'q' to quit.")

while True:
    # Display the image
    cv2.imshow('Drawing Circles', image)
    
    # Wait for a key event
    key = cv2.waitKey(1) & 0xFF
    if key == ord('q'):  # Exit if 'q' is pressed
        break

# Destroy all windows
cv2.destroyAllWindows()

