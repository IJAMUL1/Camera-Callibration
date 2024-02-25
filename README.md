# Camera Calibration using OpenCV

This project demonstrates how to perform camera calibration using OpenCV, a popular computer vision library. Camera calibration is a crucial step in computer vision applications, as it helps correct for lens distortion and obtain accurate measurements from images.

## Key Features:
- **Chessboard Calibration Pattern**: The project uses a chessboard calibration pattern to calibrate the camera. This pattern is widely used due to its well-defined corners, making it easy to detect in images.
  
- **Subpixel Refinement**: Subpixel refinement is applied to improve the accuracy of corner detection. This ensures precise localization of the chessboard corners, which is essential for accurate calibration.

- **Camera Calibration**: Using the detected chessboard corners, the project calibrates the camera to estimate intrinsic parameters such as camera matrix (`mtx`) and distortion coefficients (`dist`).

- **Reprojection Error Calculation**: After calibration, the project calculates the reprojection error to assess the accuracy of the calibration. Reprojection error measures the discrepancy between the detected image points and the corresponding reprojected points.

## Usage:
1. **Image Acquisition**: Capture multiple images of a chessboard pattern from different viewpoints using *capture_callibration_images.py*. Ensure the chessboard covers various parts of the image with varying orientations.

2. **Run Calibration Script**: Execute the provided Python script to perform camera calibration. The script reads the images, detects chessboard corners, refines them, and calculates calibration parameters.

3. **Assess Calibration Quality**: Check the mean reprojection error to evaluate the quality of the calibration. Lower values indicate better calibration accuracy.

4. **Save Calibration Results**: Save the calibration results, including the camera matrix (`mtx`), distortion coefficients (`dist`), rotation vectors (`rvecs`), and translation vectors (`tvecs`), for future use.

## Dependencies:
- Python
- OpenCV (cv2)
- NumPy

## Contribution:
Contributions, bug reports, and feature requests are welcome. Feel free to fork and submit pull requests to enhance the project.

## Acknowledgments:
- This project is based on the camera calibration techniques provided by OpenCV.
- Special thanks to the OpenCV community for their valuable contributions.

## References:
- OpenCV Documentation: [Camera Calibration](https://docs.opencv.org/4.x/d9/d0c/group__calib3d.html#ga3207604e4b1a1758aa66acb6ed5aa65d)

Feel free to customize this summary for your GitHub README file, adding any additional information or sections as needed.
