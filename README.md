#Maze Solver

#Overview

Maze Solver is a Python project that uses image processing techniques to solve a maze from an input image. By leveraging the OpenCV library, the program performs a series of operations including thresholding, contour detection, morphological transformations, and masking to identify and highlight the solution path in the maze.

#Features

Converts input maze images to binary format.

Detects and highlights maze walls and paths.

Applies dilation and erosion techniques to refine the maze paths.

Highlights the solution path on the original maze image.

#Requirements

To run this project, you need the following:

Python 3.x

OpenCV (cv2)

NumPy

#Installation

Clone the repository:

git clone <repository_url>

Navigate to the project directory:

cd Maze_solver

Install the required dependencies:

pip install -r requirements.txt

#Usage

Update the filename variable in the script to point to your maze image file:

filename = '/path/to/your/maze/image'

Run the script:

python maze_solver.py

The program will display intermediate steps in solving the maze and save the processed images in the specified folder.

#Steps in Maze Solving

Binary Conversion:
Converts the input maze image into a binary image for processing.

Contour Detection:
Identifies the contours of the maze to mark the walls and paths.

Morphological Operations:

Dilation: Enlarges the boundaries of the maze path.

Erosion: Shrinks the boundaries to refine the path.

Difference Calculation:
Finds the difference between dilated and eroded images to extract the solution path.

Masking and Path Highlighting:
Overlays the solution path onto the original maze image.

#Output

The program saves the following processed images in the specified directory:

Thresholded Image

Contours (Initial and Final)

Dilated Image

Eroded Image

Difference Image

Masked Solution Path

Final Solved Maze

#Contributing

Feel free to fork this repository, make improvements, and submit pull requests. Suggestions and issues are welcome!

#License

This project is licensed under the MIT License.

#Acknowledgements

OpenCV for its powerful image processing capabilities.

NumPy for array manipulations.


