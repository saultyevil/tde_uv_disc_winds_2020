# tde_uv_disc_winds_2020 

Data for Parkinson et al. 2020 titled "Accretion Disc Winds in Tidal Disruption 
Events: Ultraviolet Spectral Lines as Orientation Indicators". 

Please feel free to play around with the data and make your own figures. The 
spectra provided here should be machine-readable using your favourite 
programming language and functions, i.e. astropy, pandas or numpy can parse 
these files.

The Python version and git commit for each spectrum can be found at the top of 
file.

If you use any of these models, please cite the MNRAS paper!

arXiv: [blank]

## File Names

The file names should give a complete description of the model spectrum. All
models which start with "clump" indicate that the model is a clumped wind model
with a filling factor of f_v = 0.1. File names end with either "cno" or "solar"
indicating the elemental abundances which were assumed in this model. Finally,
models are either labelled as "wide-angle" or "equatorial" to indicate the
geometry of the model. 

## File Contents

The first 25 lines of each file contain the relevant metadata for each spectrum
file.

    LINES 1 - 4  :  information regarding the version of Python which the 
                    spectrum was created with. Includes the git commit and a 
                    link to GitHub repository containing the branch.

    LINES     6  :  the units of the spectrum.

    LINES 8 - 25 :  the key parameters of the model, i.e. the parameters 
                    controlling the underlying continuum and the wind geometry.

The remaining lines of the file contain the spectrum data, with the following
column headers.

    Freq.   :  the frequency bins in Hz

    Lambda  :  the wavelength bins in Angstroms

    10      :  the flux in the units defined on LINE 6 for an inclination angle 
               of 10 degrees relative to the z axis

    30      :  the flux in the units defined on LINE 6 for an inclination angle 
               of 30 degrees relative to the z axis

    45      :  the flux in the units defined on LINE 6 for an inclination angle 
               of 45 degrees relative to the z axis

    60      :  the flux in the units defined on LINE 6 for an inclination angle 
               of 60 degrees relative to the z axis

    75      :  the flux in the units defined on LINE 6 for an inclination angle 
               of 75 degrees relative to the z axis

    85      :  the flux in the units defined on LINE 6 for an inclination angle 
               of 85 degrees relative to the z axis

## Parameter Files

For those interested, the complete parameter file for each model can be found
in the "parameter_files" directory. A complete description of the input parameters can be
found as part of the standard documentation for Python.

The models were run using a fork of Python, specifically on the "tde" branch.
This version of Python can be found here,

[https://github.com/saultyevil/python/tree/tde](https://github.com/saultyevil/python/tree/tde)

The main version of Python can be found on GitHub at the following web address,

[https://github.com/agnwinds/python/](https://github.com/agnwinds/python/)

## Contact

If there are any problems, or if you have any questions, you can contact Edward
Parkinson at e.j.parkinson@soton.ac.uk.
