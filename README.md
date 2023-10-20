# heart_seg
heart segmentation code for manuscript

Usage: If videos are stable, use heartrate_calculation.ipynb to manually segment the heart region and calculate heart rate. 
If videos are not, use heart_segmentation.ipynb to stabilize and automatically segment a region around the heart.

Segmentation is based on triangulating the heart region based on the gut and eyes so as to be orientation-agnostic. dynamic background
subtraction and fourier analysis of the resulting frame-by-frame differences results in a heart rate calculation.
