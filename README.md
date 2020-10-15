# ICA_GW
Code for simulating noise removal in gravitational wave signals based on independent component analysis with particular aim of iKAGRA

# Prerequisites (vesion usued in development)
* Python3 (3.7)

You also need to prepare data files of GW strain and enviroment channels in .gwf format.

## Python modules
* LAL 
* LALframe 
* numpy
* scipy
* sklearn
* matplotlib

# Usage
By running each stage of ipython script, one can 
 - Check timelines of the data adopted in the analysis (raw and whitened),
 - See ASD and spectrogram of data.
 - Perform FastICA
 - Check mock signal
 - Parameter estimation based on mock data.

## setup & parameters
 
### data
 - `str_dir`, `env_dir`: Location of each of strain and enviroment channel data.
 - `str_root`, `env_root`: File name of each of strain and enviroment channl data.
 - `str_idx`, `env_idx`: Index of each of strain and enviroment channel data.
 - `outdir`, `outroot`: Location and file name of results.
### mock signal (burst-like)
 - `amp`: (Dimensionless) amplitude of mock signal
 - `duration`: Duration of mock signal
 - `fudge_gamma`: Decay rate of signal
 - `fudge_omega`: Frequency of signal
