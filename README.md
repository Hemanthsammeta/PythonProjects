# OpenCV Circle Drawing with Mouse Clicks

This Python project demonstrates how to use **OpenCV** to draw circles on an image in real-time whenever a user clicks the mouse. It's a beginner-friendly project to get familiar with OpenCV's GUI event handling and image manipulation.

## Features
- Draw circles at the exact point where the user clicks.
- Customize circle size and color.
- Interactive and real-time updates.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [How It Works](#how-it-works)
- [Project Structure](#project-structure)


## Installation

1. **Clone this repository**:
   ```bash
   git clone https://github.com/yourusername/opencv-circle-drawing.git
   cd opencv-circle-drawing
2. **Install dependencies**:
   pip install -r requirements.txt
   pip install opencv-python

## Usage
1. **Run the Python script**:
    python draw_circles.py
2.**Controls**:
    Click anywhere on the window to draw a circle at the clicked location.
    Press the Esc key to close the window.

## How It Works
  .The project uses OpenCV's cv2.setMouseCallback() function to detect mouse clicks.
  .Upon a mouse click, the program captures the (x, y) coordinates of the click.
  .A circle is drawn at the captured coordinates using cv2.circle().
  .The image is updated in real-time to reflect the drawn circles.

## Project Structure
  opencv-circle-drawing/
│
├── draw_circles.py       # Main Python script
├── requirements.txt      # Dependencies
├── README.md             # Project documentation
└── .gitignore            # Ignored files
