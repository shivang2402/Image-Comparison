# Image-Comparison
Image Comparison and Alignment with Different Techniques<br><br>

This repository contains two Python scripts that enable you to compare and align two images using different techniques for image analysis and processing. Both scripts perform the task of image comparison and alignment, but they utilize distinct algorithms. Here's an overview of the two implementations:<br>

**Implementation 1: Feature Detection and Matching with SIFT**<br>

The first implementation utilizes the Scale-Invariant Feature Transform (SIFT) algorithm for feature detection and matching. The steps involved in this implementation include:<br>

1.Load the two images to be compared.<br>
2.Perform feature detection and matching using SIFT.
3.Apply a ratio test to filter the good matches.<br>
4.Extract keypoints from the good matches.<br>
5.Estimate the transformation matrix using the Random Sample Consensus (RANSAC) algorithm.<br>
6.Align the first image with the second image using the estimated transformation matrix.<br>
7.Perform histogram matching to adjust for differences in lighting and intensity.<br>
8.Calculate the absolute difference between the aligned image and the second image.<br>
9.Denoise the difference image and threshold it to identify significant differences.<br>
10.Find contours of the significant differences and filter small boxes.<br>
11.Draw non-overlapping bounding boxes on the second image to highlight the differences.<br>
12.Display a side-by-side comparison of the first image and the highlighted differences.<br><br>
**Implementation 2: Optical Flow with Lucas-Kanade Algorithm**<br>

The second implementation utilizes the Lucas-Kanade optical flow algorithm for image comparison and alignment. The steps involved in this implementation include:<br>

1.Load the two images to be compared.<br>
2.Convert the images to grayscale for optical flow analysis.<br>
3.Perform optical flow using the Lucas-Kanade algorithm.<br>
4.Filter and create keypoints based on the detected optical flow.<br>
5.Estimate the transformation matrix using the Random Sample Consensus (RANSAC) algorithm.<br>
6.Align the first image with the second image using the estimated transformation matrix.<br>
7.Perform histogram matching to adjust for differences in lighting and intensity.<br>
8.Calculate the absolute difference between the aligned image and the second image.<br>
9.Denoise the difference image and threshold it to identify significant differences.<br>
10.Find contours of the significant differences and filter small boxes.<br>
11.Draw non-overlapping bounding boxes on the second image to highlight the differences.<br>
12.Display a side-by-side comparison of the first image and the highlighted differences.<br><br>
These two implementations offer different approaches for image comparison and alignment, allowing you to choose the technique that best suits your specific requirements. <br>
