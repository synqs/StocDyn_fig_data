# StocDyn_fig_data
Here we provide the data and jupyter notebooks to generate the figures of the paper "Stochastic dynamics of a few sodium atoms in a cold potassium cloud". arXiv:2101.01135

Each figure has its own Notebook. For some figures digitized data is needed. We, therefore, provide the raw data and the notebook containing the digitization routine to generate the digitized data.

## Figure1&4B: Time trace of (digitized) sodium and potassium
The notebook generates the digitized sodium data from the raw data. One time trace of sodium is plotted  with overlaying digitized time trace and the belonging potassium data.

#### Sodium and Potassium:
dataset : September 24, 2020 with potassium
exposure time: 75 ms
time between images : 12 ms
number of images in each reference wing: 100
filename:

#### Further data for digitization calibration:
dataset : September 24, 2020 without potassium
exposure time: 75 ms
time between images : 12 ms
number of images in each reference wing: 100
filename:

## Figure 5: Characterization  of  atom  number  fluctuations  for sodium and potassium
The notebook plots the loading for sodium/potassium together with the average and error band. Bootstrapping is used to get the variance for variance/mean plots.

#### Sodium:
dataset : October 7th, 2020
exposure time: 200 ms
time between images : 12 ms
number of images in each reference wing: 100
filename:
#### Potassium:
dataset : October 15th, 2020
exposure time: 100 ms
time between images : 12 ms
number of images in each reference wing: 100
filename:


## Figure 6:  Accurate atom counting of sodium
The notebook plots the histogram, which is used to extract calibration factor. Data is digitized and plotted together with the calibrated data.

#### Sodium
dataset : October 17th, 2020 
exposure time: 200 ms
time between images : 12 ms
number of images in each reference wing: 100
filename: 

## Figure 7: Counting  statistics  of  sodium  with  and  without potassium  atoms  present
The notebook extracts the calbration factor needed for the digitization routine. Digitized data is loaded and number of single atom jumps up and down are extracted. Bootstrapping is used to calculate mean and std.

dataset : September 24, 2020 with and without potassium
exposure time: 75 ms
time between images : 12 ms
number of images in each reference wing: 100
filename:



