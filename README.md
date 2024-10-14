## README for Axion Form Factors Data

This repository provides the axion form factors A and B for the KSZV and DFSZ models at finite nuclear density. The data is available in `.txt` format, where each row corresponds to a combination of nucleon densities, momenta, and axion energies. Below, we describe the contents of the files and how the data is organized.


## Files Provided

- KSZV Axion Form Factors:
  - `A.txt`: Form factor A for the KSZV axion model.
  - `B.txt`: Form factor B for the KSZV axion model.
  
- DFSZ Axion Form Factors:
  - `A_DFSZ.txt`: Form factor A for the DFSZ axion model.
  - `B_DFSZ.txt`: Form factor B for the DFSZ axion model.
  
Each file contains the form factors as a function of neutron density, proton density, axion energy, and the magnitude of the nucleon momentum and cosine of the angle between axion and nucleon momentum. For the DFSZ axion model files, an additional parameter \sin(\beta)^2 is provided.


## Data Format

In each file, the rows contain the following entries (from left to right):

1. Neutron Density: Neutron density in units of nuclear saturation density.
2. Proton Density: Proton density in units of nuclear saturation density.
3. Axion Energy: Axion energy in [MeV].
4. Nucleon Momentum: Magnitude of the nucleon momentum in [MeV].
5. Cosine of the angle between axion and nucleon momentum.
6. \sin(\beta)^2 Parameter (Only for DFSZ files): Value of the parameter \sin(\beta)^2.
7. Mean Axion-Proton Form Factor: Mean value of the axion-proton form factor.
8. Upper Error Band (Proton Form Factor): Upper value of the error band for the axion-proton form factor.
9. Lower Error Band (Proton Form Factor): Lower value of the error band for the axion-proton form factor.
10. Mean Axion-Neutron Form Factor: Mean value of the axion-neutron form factor.
11. Upper Error Band (Neutron Form Factor): Upper value of the error band for the axion-neutron form factor.
12. Lower Error Band (Neutron Form Factor): Lower value of the error band for the axion-neutron form factor.

Note that the values for the Error Bands are only estimates here and can differ slightly from the ones shown in the corresponding publication.


The form factors are provided by varying five key parameters in the following order (going down the columns):

1. Neutron Density: 9 discrete values {0., 0.3, 0.6, 0.9, 1.2, 1.5, 1.8, 2.1, 2.4}
2. Proton Density: 9 discrete values {0., 0.3, 0.6, 0.9, 1.2, 1.5, 1.8, 2.1, 2.4}
3. Axion Energy: 8 discrete values {0.1, 50, 100, 150, 200, 250, 300, 350}
4. Neutron Momentum: 8 discrete values {0.1, 50, 100, 150, 200, 250, 300, 400} 
5. Cosine of angle between nucleon and axion momentum: 7 discrete values {-0.9, -0.6, -0.3, 0, 0.3, 0.6, 0.9}
6. \sin(\beta)^2 Parameter (only in DFSZ files): 4 discrete values {0, 0.1, 0.5, 1}

## Usage

To efficiently read in the values and understand the data, iterate over the columns in the order of the six varying parameters listed above. Each row in the files provides the form factors for one specific combination of these parameters. 

For precise scientific use, ensure to account for both the mean values and the error bands of the form factors.


## Citation

If you use this data in your research, cite the corresponding publication.

