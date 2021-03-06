# Pantheon
For a quick run:
To set this up in Cosmomc, see the in file in the ini folder or set things up as if you were running with JLA, but add these three lines:

jla_dataset=/your-path/full_long.dataset
param[alpha_JLA]=0.0
param[beta_JLA]=0.0

The alpha and beta are just dummy values since they are not used here.  The purpose is just to fix them.
-----

AAA_README   data_fitres        ini_example            PLOTS    sim_fitres    sys_full_long.txt
AAA_README~  full_long.dataset  lcparam_full_long.txt  SCRIPTS  spec_summary

Full readme:

-> A table of the spectroscopic observations of each SN in the PS1 sample that includes their ID, date of observation, telescope observed and measured redshift.
Folder: spec_summary/

->A table of key recovered parameters from the light-curve fits for the full Pantheon sample.
lcparam_full_long.txt have redshifts and distances and sys_full_long.txt has systematics.  

->We also include a full output table from the SNANA fitter of a thorough listing of fitted parameters and other properties of the light-curves.
Folder: data_fitres/

->A table of binned distance estimates over redshift for a compressed version of the dataset
Folder: Binned_data/

->A full systematic covariance matrix for the binned and unbinned versions.
The sys_full_long.txt has first line that says number of SNe then has # by # rows that can be read into a matrix.

->Stellar catalogs of the MD fields.

->Necessary files to use with the CosmoMC or CosmoSIS software with instructions.
See the ini_example/ and the .dataset file included

-> A folder of all the SNANA set-up scripts to fit each sample. A folder of all the SNANA set-up scripts to simulate each sample.
This is included in the SNANA release of this data that can be grabbed by downloading http://snana.uchicago.edu/

-> Output tables for 30 simulated samples used to test external methods on perform null tests on this dataset.
See the sim_fitres/ folder

->Code for remaking all figures in this paper.
See the SCRIPTS/ folder

->Plots
See the Plots/ folder