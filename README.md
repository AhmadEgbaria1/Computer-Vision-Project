#3D Vision Project README
This notebook contains the solution for Homework 2 of the University of Haifa's Computer Vision course, focusing on 3D Vision concepts.

Project Structure:
The project is divided into three main parts, each addressing a specific aspect of 3D vision and multi-view geometry.

Part 1 - Constraining Putative Matches Using Geometry
Objective: To understand and apply epipolar geometry to filter feature matches between image pairs.

Tasks:

Obtain SIFT-based matches: Compute SIFT features and perform matching between two images.
Visualize a set of matches: Display the image pair with lines connecting matching points.
Recover the Epipolar geometry: Estimate the Fundamental matrix (F) from the matches.
Visualize the Epipolar geometry: Display epipolar lines based on the calculated Fundamental matrix.
Constrain a set of matches: Filter initial matches using the epipolar constraint derived from F.
Part 2 - Middle-View Synthesis from a Rectified Stereo Pair
Objective: To synthesize an intermediate view from a rectified stereo pair using two different strategies.

Strategies:

Strategy A: Via Photometric Stereo (Dense Disparity Map)
Compute a dense disparity map.
Use the disparity map to synthesize the central image.
Discuss the challenges and solutions for this approach.
Strategy B: Via Sparse Reconstruction (Triangulation and Warping)
Obtain geometry-constrained matches.
Use triangulation to find interest points in the new central image.
Subdivide the image into triangular regions and warp content from input images to the target.
Discuss the challenges and solutions for this approach.
Part 3 - Motion Segmentation
Objective: To segment feature matches into 'static' (background), 'dynamic' (moving object), or 'outliers' given a pair of images with a single moving object.

Tasks:

Utilize functions developed in Part 1.
Process image pairs from data/pairs_to_segment (including custom pairs).
Visualize 'outlier', 'static', and 'dynamic' matches separately.
