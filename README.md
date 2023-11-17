# Brain-Segmentation-MRI-Preprocessing
Preprocessing Pipeline Read Me

Introduction: 

This preprocessing pipeline is designed to perform various steps on neuroimaging data, specifically structural MRI scans from the BraTS (Brain Tumor Segmentation) dataset. The pipeline includes normalization, adaptive histogram equalization, noise reduction, and registration to a standard template.

Components:

1. Data Loading
Purpose: Load the input structural MRI scan.
Usage: Replace input_path with the path to the structural MRI scan you want to process.
2. Normalization to Range [-1, 1]
Purpose: Normalize the image intensity values to the range [-1, 1].
Usage: Apply the normalization process to enhance comparability between different scans.
3. Adaptive Histogram Equalization
Purpose: Enhance contrast and improve visibility of details.
Usage: Apply adaptive histogram equalization to the normalized data.
4. Noise Reduction (Gaussian Filter)
Purpose: Reduce noise in the image.
Usage: Apply a Gaussian filter to the data for noise reduction.
5. Resampling to Standard Template
Purpose: Resample the preprocessed image to a standard template (MNI152).
Usage: Compare the preprocessed image with the template for standardization.
6. Structural Image Display
Purpose: Display the original and preprocessed images for visual inspection.
Usage: Execute the corresponding code blocks to visualize the images.

Data Loading and Preprocessing:

Modify the input_path variable to point to the desired structural MRI scan.
Execute the code blocks for data loading, normalization, histogram equalization, and noise reduction.

Resampling and Standardization:

Execute the code blocks for resampling the image to the MNI152 template.
Affine and Nonlinear Registration:

Execute the code blocks for affine and nonlinear registration using FLIRT and FNIRT.
Display Results:

Execute the code blocks for displaying original, preprocessed, and warped images.

Dependencies:
nibabel
numpy
matplotlib
nilearn
fslpy
ants
nipype

Conclusion
This preprocessing pipeline provides a comprehensive set of steps to enhance, standardize, and align structural MRI scans for further analysis or comparison.

