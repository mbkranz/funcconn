# funcconn
these scripts are used to concatenate functional connectivity data processed from CPAC and create graph theory metrics from these data

### make_corticalmorph_dfs.ipynb
- this notebook (1) concatenates preprocessed freesurfer data (i.e., resampled to fsaverage and smoothed for each subject), (2) adds annotation network labels (currently using the Yeo 7 Network annotation but can use any annotation file), and (3) filters by network and saves in pickle file
- in a last part of this notebook, also loads the wholebrain fsaverage pickle file and calculates the wholebrain (ie., cortex) measures (surface area and thickness).

### run_statmodels.ipynb
- creates csv files of different node specific metrics (for each individual) and individual summary specific metrics (for each individual). This is done by integrating functions from brainx, networkx, and pandas.
