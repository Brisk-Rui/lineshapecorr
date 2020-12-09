# lineshapecorr
line shape correction scheme for correcting distorted infrared (IR) spectra. The measured IR absorption spectra are real valued. Since the line shape is a linear combination of the real and imaginary parts, we have to retrieve the imaginary part. We do this by first FT to time domain and forcing causality by taking only the positive times. Enforcing causality is equivalent to the KK relation. By FT back to the frequency domain we now have a complex function. We adjust the linear combination of the real and imaginary parts by introducing a phase factor. Phase is then varied to find the most symmetric line shape. 

"""
Created on Wed Dec 9 2020
Phase correction for distorted line shapes observed on infrared (IR) absorption spectra
Based on the work of: 
Gökçen Tek and Peter Hamm; A Correction Scheme for Fano Line Shapes in Two-Dimensional Infrared Spectroscopy.
https://doi.org/10.1021/acs.jpclett.0c01752
@author: zaphodcuk
"""


