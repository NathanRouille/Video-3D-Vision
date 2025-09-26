## Lab 1: Motion Estimation — Block Matching and Optical Flow
- **Objective**: Implement and compare block-matching and optical-flow methods for estimating motion between frames, and evaluate their effect on motion compensation.
- **Key Topics**:
  - Block matching with SSD/SAD metrics and regularization with neighbor predictors.
  - Influence of block size, search radius, and regularization weight.
  - Horn–Schunck optical flow and impact of smoothness and iteration parameters.
  - Motion compensation and evaluation with PSNR.
- **Skills Applied**:
  - Implementation of block-matching and regularized variants.
  - Construction of dense motion-compensated frames and PSNR evaluation.
  - Implementation of Horn–Schunck optical flow and initialization strategies.
  - Experimental comparison of block-matching vs optical flow on different sequences.


## Lab 2: Parametric Motion Estimation
- **Objective**: Estimate global motion between two images using direct Fourier-based methods and indirect approaches such as block matching and optical flow, and compare their robustness.
- **Key Topics**:
  - Phase-based translation estimation in the Fourier domain.
  - Indirect estimation from motion vector fields (block matching, Horn–Schunck optical flow).
  - Comparative evaluation under noise, periodicity issues, and sub-pixel displacements.
- **Skills Applied**:
  - Implementation of Fourier-based translation estimation.
  - Application of block matching and optical flow for parametric motion.
  - Quantitative and qualitative comparison of estimation accuracy and robustness.
 
## Lab 3: Kalman Filter and Multi-Object Tracking
- **Objective**: Implement and analyze the Kalman filter for state estimation in 1D and apply it to multi-object tracking using a tracking-by-detection approach.
- **Key Topics**:
  - Gaussian distributions and update rules via product of Gaussians.
  - Kalman filter prediction and update steps for position–velocity models.
  - Multi-object tracking with SORT: state definition, IOU-based association, and Hungarian algorithm.
- **Skills Applied**:
  - Implementation of Kalman filter in 1D and extension to bounding-box tracking.
  - Integration of detection and tracking for multi-object scenarios.
  - Practical understanding of uncertainty reduction and identity preservation in MOT.

## Lab 4: Particle Filter for Object Tracking
- **Objective**: Implement a particle filter for single-object tracking using color-based appearance models.
- **Key Topics**:
  - Appearance models: pixel-wise MSE and HSV histogram comparison.
  - Particle filter: state propagation, weight update, and resampling.
  - Tracking objects with non-constant velocity in videos.
- **Skills Applied**:
  - Implementation of particle filter with generic state and measurement models.
  - Design of robust appearance models for visual tracking.
  - Integration of prediction, update, resampling, and state estimation.

## Lab 5: Homography Estimation and Panorama Stitching
- **Objective**: Estimate homographies between images using the DLT algorithm and improve robustness with RANSAC for applications such as document rectification and panorama creation.
- **Key Topics**:
  - Direct Linear Transform (DLT): normalization, matrix construction, SVD, and discussion of required keypoints and degrees of freedom.
  - Sensitivity of DLT to noise and outliers in point correspondences.
  - Robust homography estimation with RANSAC.
  - Automatic keypoint detection and matching with SIFT and BRISK descriptors.
  - Panorama stitching and handling illumination differences between images.
- **Skills Applied**:
  - Manual and automatic selection of keypoints.
  - Implementation of DLT and RANSAC for homography estimation.
  - Use of OpenCV for keypoint detection, matching, and image warping.
  - Practical construction of document rectification and panoramas.

## Lab 6: Camera Calibration with Chessboard Patterns
- **Objective**: Implement a complete camera calibration pipeline using chessboard images and compare the results with OpenCV’s built-in calibration function.
- **Key Topics**:
  - Homography estimation with DLT and its role in calibration.
  - Computation of the intrinsic matrix using Zhang’s method.
  - Recovery of extrinsic parameters (rotation and translation).
  - Modeling and correction of lens distortion (radial distortion).
- **Skills Applied**:
  - Implementation of camera calibration algorithms in Python and OpenCV.
  - Application of linear algebra techniques (SVD, orthogonality constraints, Cholesky).
  - Estimation of both intrinsic and extrinsic parameters from real data.
  - Distortion correction and evaluation of projection error.
  - Critical comparison between a manual implementation and library functions.

