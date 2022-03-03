# Aligning_Defocus_series(TEM)

This is a MATLAB script to align Stack-TEM images by applyng Contrast stretching, Gaussian filtering, Tight masking, and COM method.

Brifely, the process of masking has a procedure:
  1. Contrast stretching To TEM images to distinguish a target and boundary more clearly.
  2. Gaussian filtering to the result of "1." to neglect the effect of diffraction so that there is no dark-cross line inside a target.
  3. Tighit Masking
  4. COM align (Center-of-mass align) to the masking result. During this process, we can find how we have to shift each images to make the center of the target at the center of the image window.
  5. with the 

Ofcourse, since the contrast of TEM images is not linear(For example, diffraction pattern at target's boundary)
