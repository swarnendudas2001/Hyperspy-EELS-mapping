# Hyperspy-EELS-mapping
Low loss EELS mapping (peak postion, peak intensity and thickness map from zero-loss intensity)

# Parameters used in the functions
e_axis_start: starting value of our energy range of interest (in eV)
e_axis_end: ending value of our energy range of interest (in eV)
roi_size: edge length of our square region of interest (in pixels)
roi_x: x-coordinate of the origin (top-left corner) of our square region of interest
roi_y: y-coordinate of the origin (top-left corner) of our square region of interest
x: x dimension of our spectrum image (in pixels)
y: y dimension of our spectrum image (in pixels)
save_dir: location of folder to save the output figures

# Function to sum spectra from each pixel of a region of interest (ROI) in the spectrum image 
To increase signal-to-noise ratio

# Function to sum spectra from each pixel of a region of interest (ROI) in the spectrum image & fit specific peaks in the summed spectrum #
Here we fitted two peaks (plasmonic extinctions & interband transitions) with Gaussian

# Function for Low spacial resolution mapping of the peak position and intensity with the fitted peaks
For quick verification of quality of curve fitting and spacial resolution limited by the choice of ROI size.

# Function for High spacial resolution (using rolling average) mapping of the peak position and intensity with the fitted peaks
High spacial resolution map for the final figures after optimizing the ROI size with the quicker scan. This step is time-expensive.

# Function for High spacial resolution (using rolling average) mapping of the intensity in the fitted zero-loss peak (ZLP)
For thickness map

# Function to sum spectra from each pixel of a region of interest (ROI) in the spectrum image, fit specific peaks in the summed spectrum and output the fitted spectrum plot while the ROI scans the spectrum image
To check how good the curve fitting is in different regions of the spectrum image for a particular ROI size. The quality of curve fitting can change based on difference in signal-to-noise ratio, which can be optimized by ROI size.
