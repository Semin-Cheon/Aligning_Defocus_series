# Aligning_Defocus_series(TEM)

This is a MATLAB script to align Stack-TEM images by applyng Contrast stretching, Gaussian filtering, Tight masking, and COM method.

Brifely, the process follows the procedures in bellow:
  1. Contrast Inversion to each TEM images
  2. Contrast stretching To TEM images to distinguish a target and boundary more clearly.
  3. Gaussian filtering to the result of "1." to neglect the effect of diffraction so that there is no dark-cross line inside a target.
  4. Tighit Masking
  5. COM align (Center-of-mass align) to the masking result. During this process, we can find how we have to shift each images to make the center of the target at the center of the image window (Named "Shift Coefficient").
  6. with the Shift Coefficients, move raw TEM images.

