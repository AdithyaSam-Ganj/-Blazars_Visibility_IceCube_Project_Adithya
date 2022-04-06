# Blazars_Visibility_IceCube_StudentProject_Adithya


# Testing Blazar Sky Visible to IceCube 

## Project Outline 
 The project was inspired by 2 papers by Murase(https://journals.aps.org/prd/abstract/10.1103/PhysRevD.90.023007) and Padvoni(https://arxiv.org/pdf/1506.09135.pdf).
They suggest a relation between the neutrinos emitter from the synchrotron peak of a blazar and the enrgy of the synch. peak.
We have studied if these predictions can explain the ASTRONOMICAL neutrino detected at IcuCube. But this project is not limited to these 2 papers.The main aim of the project is listed below.

AIM :
1. Main aim of the project is to see which class of blazars IceCube is more sensitive to
2. Compare the visibility diff. sub-classes of blazars  (LSP, ISP, HSP;   BL Lacs, FSRQs). 
3. Extend the prediction to higher energies by using IceCube Gen2 sensitivity 

We are considering 2 seperate catalogues(3HSP and RomaBZcat), the code for both of them are written in seperate jupiter notebooks. We have used X-Ray, Gamma Ray and Synchrotron Peak energy 
data separately and tried to corellated them with IceCube sensitivity.
## Catalogues 
The main catalogues used are 3HSP, 4fgl and RomaBZCat.
The code written for 3HSP and 4FGL are in seperate
jupiter notebooks. The different notebooks will be refered to as 3HSPN and 4FGLN from here on in the read me file.    


List of Catalogues used for this project :

The 4fgl catalogue has been stored in 3 differnt catalogues.
1. 4fgl.csv  
2. 4fgl_.csv
3. 4fgl_alotmore.csv

4. 3hsp.csv - 3HSP catalogue 

IceCube sensitivity plots from the paper https://arxiv.org/pdf/1910.08488.pdf

5. e3_sensitivity.csv
6. e2_sensitivity_datapoints.csv
7. 3cubed_90.csv
8. esquared_90.csv



IceCube effective area as a function of neutrino energy is stored in the following catalogues. (https://arxiv.org/pdf/1910.08488.pdf)
The declination values are mentioned in the the .csv files. 

9. a30-85.csv - 30 to 80 degrees
10. an5-30.csv - minus 5 to 30 degrees 
11. an30n5.csv - minus 30 to minus 5 degrees 
12. an90n30.csv - minus 90 to minus 30 degrees


Data from the RomaBZCat catalogues is stored in the following set of catalogues 

13. romabzcat_full.csv - The entire romabzcat catalogue 
14. BZcat_only_classification.csv - List of the classification for all the sources in romabzcat_full.csv



## Code 

The project is divided into two jupiter notebooks that each deal with separate blazar catalogs, 3HSP and RomaBZcat. We have done a similar analysis on both catalogs.
The main functions defined in the programma are

1. FSRQ_Blazarzone - To calculate the energy of the neutrinos from the blazar zone. Refer slide no 24 

2. FSRQ_Blr - To calculate the energy of neutrino sed peak from BLR regions.Refer to slide number 24 in - Adithya_prelim_results.pdf

3. BL_Lac - Energy of neutrino SED peak is obtained from sync. peak energy. Refer to slide number 23 in - Adithya_prelim_results.pdf

4. frame_conversion - used to convert energy from one frames to the other. 

5. crossmatch_tree - This function is used to cross match sources between two different catalogs. It takes two arrays and the minimum radius between the sources are the input. The output is an array of index of matched and unmatched sources. 

6. neutrino_flux - https://arxiv.org/pdf/1810.08482.pdf . Equation 4

7. neutrino_flux2 - https://arxiv.org/pdf/1810.08482.pdf . Equation 7 

8. FindSorted , FindSorted1 - This function is used to find the effective area of icecube for a given source depending on the declination and the 



The methods we have considered to estimate neutrino flux from gamma-ray flux and X-ray flux are available in the presentation Adithya_prelim_results.pdf.
