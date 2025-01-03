# Face Recognition System: Eigenfaces vs. Fisherfaces
  This repository contains the implementation of a Face Recognition System where two popular methods, Eigenfaces and Fisherfaces, are compared for their effectiveness in recognizing faces under varying conditions.
  The project showcases the application of Principal Component Analysis (PCA) and Linear Discriminant Analysis (LDA) for dimensionality reduction and class separability, respectively.

# Key Features
  Eigenfaces Method:
   * Uses PCA to reduce the dimensionality of facial images.
   * Captures the most significant eigenvectors (Eigenfaces) to represent face data.
   * Projects test images onto the Eigenface space and calculates similarity for recognition.
     
  Fisherfaces Method:
  * Combines PCA and LDA for enhanced class separability.
  * Projects images onto an optimal subspace that maximizes between-class scatter while minimizing within-class scatter.
  * Designed to perform well in scenarios with varying lighting and expressions.

# Comparison:
  Both methods are evaluated for accuracy, and their performance is compared under the same dataset and conditions.

# Tools & Technologies
  * Python: Core programming language for implementation.
  * NumPy: For efficient numerical computations.
  * OpenCV: For face detection using Haar cascades.
  * PIL: For image preprocessing.
  * Scikit-learn: For data splitting and utility functions.

# Workflow
  Data Preprocessing: 
    * Face images are cropped and converted to grayscale.
    * Images are flattened into vectors for processing.
    
  Training:
    * Eigenfaces: PCA is applied to compute eigenvalues and eigenvectors.
    * Fisherfaces: PCA is followed by LDA to achieve optimal subspace projection.
    
  Testing:
    * Test images are projected onto the respective subspaces (Eigenface or Fisherface).
    * Closest matches are identified using distance metrics.
    
  Performance Evaluation:
    Accuracy of both methods is calculated and printed for comparison.
