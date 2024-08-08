# Air-Canvas

## Project Overview

This project is an interactive drawing application that leverages computer vision to create a real-time painting experience. By using a webcam to track a colored marker, users can draw directly onto a virtual canvas displayed on their screen. The application allows for dynamic color selection and canvas management, making it a versatile tool for digital drawing and art.

## Key Features

- **Real-Time Drawing**: Users can draw on a virtual canvas by moving a colored marker in front of their webcam.
- **Color Selection**: Choose from four predefined colors (Blue, Green, Red, Yellow) to draw with.
- **Canvas Clearing**: Easily clear the entire canvas with a dedicated "CLEAR ALL" button.
- **Customizable Marker Detection**: Adjust HSV (Hue, Saturation, Value) thresholds via trackbars to match different marker colors and lighting conditions.

## How It Works

1. **Marker Detection**:
   - The application uses OpenCV to capture video from the webcam.
   - The captured frames are converted to HSV (Hue, Saturation, Value) color space to detect the colored marker.
   - HSV thresholds can be adjusted in real-time using trackbars to ensure accurate marker detection.

2. **Drawing Mechanism**:
   - When the marker is detected, its position is used to draw on the canvas.
   - Users can switch between drawing colors by clicking on color buttons displayed on the screen.

3. **Canvas Management**:
   - The virtual canvas is initialized as a white background.
   - The "CLEAR ALL" button allows users to reset the canvas by erasing all drawn content.
