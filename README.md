# SWBio_CD_assessment

## CD DATA PROCESSING AND PLOTTING 

This script uses python to take a set of raw circular dichroism data (uploaded by the user as .txt files). 
The input dataset will be converted into MRE (mean residue ellipticity), normalised against a blank run using only buffer, and plotted to allow for a comparison of protein folding before and after heating to 95 degrees celsius.
A plot of the HT values will also be produced for reference. 
This script can be applied to CD data consisting of pre&postmelt measurements, as well as melting and cooling experiments between 5-95 degrees.

To run this script:
    1. Ensure that the required modules are installed (instructions for this can be found below)
    2. Download the script along with the example data files into the same directory. 
    3. The values for the cell pathlength, protein concentration, no. of peptide bonds and melt wavelength are present in the script, however users using different experimental parameters should enter these before running. The axes limits were input to be optimised for the example parameters. Therefore, edit these if the edited parameters produce spectra which do not suitably fit onto the plot.
    4. Input the preferred name of the file the plot will be stored in where indicated in the script. 
    5. Run the script using the example data.

This should produce a set of 4 plots:
    - In the example data, the top-left plot should show a CD curve with minima at 208 and 222nm, indicative of a strongly folded alpha helical protein both before and after melting. 
    - The top-right panel shows that the protein remains folded as an alpha helix up to 95 degrees, with little change in helicity during melting and cooling.
    - The bottom two panels should show that the HT value remains stable (apart from below 210nm wavelength in the bottom-right panel, as expected)

modules required for this script:
    - NumPy (documentation: https://numpy.org/install/)
    - matplotlib (documentation: https://matplotlib.org/stable/install/index.html)
to install these using conda: use the command in your environment 
    conda install numpy 
to install these using pip: use the command in your environment
    pip install numpy
