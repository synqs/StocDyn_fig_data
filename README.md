[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/synqs/StocDyn_fig_data/HEAD)
.. image:: https://mybinder.org/badge_logo.svg
 :target: https://mybinder.org/v2/gh/synqs/StocDyn_fig_data/HEAD
# StocDyn_fig_data
Here we provide the data and jupyter notebooks to generate the figures of the paper "Stochastic dynamics of a few sodium atoms in a cold potassium cloud". arXiv:2101.01135

Each figure has its own Notebook. For some figures digitized data is needed. We, therefore, provide the raw data and the notebook containing the digitization routine to generate the digitized data.

## Generate digitized csv
The notebook generated the digitized data from the raw data. Information needed about the datasets are
- time_between_atom_images: time between images = 12ms (for all datasets)
- Cam_EXPOT: camera exposure time = 75-200ms (depending on the dataset)
- one_atom_signal: Calibration factor extracted from histogram in each notebook corresponding to the figure
- number_of_images_without_atoms: number of images in each reference wing = 100 (for all datasets)

## Figure1&4B: Time trace of (digitized) sodium and potassium
The notebook generates the digitized sodium data from the raw data. One time trace of sodium is plotted  with overlaying digitized time trace and the belonging potassium data.

#### Sodium:
- dataset : September 24, 2020 with potassium
- exposure time: 75 ms
- time between images : 12 ms
- number of images in each reference wing: 100
- filename: Sep24_Scan_0001_use_K=True
###### Additional data used for digitization:
- dataset : September 24, 2020 without potassium
- exposure time: 75 ms
- time between images : 12 ms
- number of images in each reference wing: 100
- filename: Sep24_Scan_0001_use_K=False

#### Potassium:
- dataset : September 24, 2020 with potassium
- exposure time: 75 ms
- time between images : 12 ms
- number of images in each reference wing: 100
- filename: Sep24_K_Scan_0001_use_K=True

#### Further data for digitization calibration:
- dataset : September 24, 2020 without potassium
- exposure time: 75 ms
- time between images : 12 ms
- number of images in each reference wing: 100
- filename: Sep24_Scan_0001_use_K=False

## Figure 5: Characterization  of  atom  number  fluctuations  for sodium and potassium
The notebook plots the loading for sodium/potassium together with the average and error band. Bootstrapping is used to get the variance for variance/mean plots.

#### Sodium:
- dataset : October 7th, 2020
- exposure time: 200 ms
- time between images : 12 ms
- number of images in each reference wing: 100
- filename: Oct07_Scan_0000_Cam_EXPOT=0.2
#### Potassium:
- dataset : October 15th, 2020
- exposure time: 100 ms
- time between images : 12 ms
- number of images in each reference wing: 100
- filename: Oct15_K_Scan_0009_KtwoDInt=1.4


## Figure 6:  Accurate atom counting of sodium
The notebook plots the histogram, which is used to extract the calibration factor. Data is digitized and plotted together with the calibrated data.

#### Sodium
- dataset : October 7th, 2020
- exposure time: 200 ms
- time between images : 12 ms
- number of images in each reference wing: 100
- filename: Oct07_Scan_0000_Cam_EXPOT=0.2

## Figure 7: Counting  statistics  of  sodium  with  and  without potassium  atoms  present
The notebook extracts the calbration factor needed for the digitization routine. Digitized data is loaded and number of single atom jumps up and down are extracted. Bootstrapping is used to calculate mean and std.

#### Sodium:
- dataset : September 24, 2020 with and without potassium
- exposure time: 75 ms
- time between images : 12 ms
- number of images in each reference wing: 100
- filename: Sep24_Scan_0001_use_K=True, Sep24_Scan_0001_use_K=False
