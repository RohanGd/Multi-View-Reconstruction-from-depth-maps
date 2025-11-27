# 3dCV-projekt Point Cloud Generation

8 distorted images were given and 7 features (same, but randomly shuffled) were given for each view. Along with this camera intrinsics were given and the distortion params as well. The depth images were also given.

Step 1.
Undistort the images (see the jupyter notebook for implementation details) and inverse Sampling

Step2. 
For each feature in the view, using epipolar geometry find correspondences between the given features.

Step3.
Perform triangulation using correspondences and get 3d points for the features.

Step4.
Use scale from depth images to get actual 3d points for all pixels and create 3d point cloud.

