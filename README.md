# Computer_Vision_2
Edge Detection using Sobel Filter

Overview
This project explores edge detection using the Sobel filter on a given image. It analyzes the impact of filter size (3x3, 15x15, 31x31) on edge detection, showing how smaller filters detect fine details, while larger filters highlight prominent edges but lose finer details like pavement boundaries.

Methodology
Preprocessing
Load the input image and convert it to grayscale.
Normalize the image if required.
Sobel Filter Application

Apply the Sobel filter to detect edges using different kernel sizes:
3x3: Captures fine edges.
15x15 / 31x31: Captures larger edges while ignoring small details.
Compute gradient magnitude and direction for edge detection.
Analysis of Edge Angles

Major edge directions observed: 0°, 45°, 85°, 135°.
Histogram Analysis: Larger filters detect a wider range of edge angles compared to smaller filters.

Observations
3x3 Filter
Detects smaller edges, including fine textures.
Maximum number of pixels with an edge angle of 0° exceed 20,000.
Larger Filters (15x15, 31x31)
Detect prominent edges while ignoring small textures (e.g., pavement boundaries).
Histogram of edge angles shows detection of a wider variety of angles.

Requirements
Python 3.x
OpenCV (cv2)
NumPy
Matplotlib (for visualization)
