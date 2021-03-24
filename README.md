# BIDS-helper-scripts
Scripts with functions that could be re-used for future BIDS formatting efforts 

## pydeface 

- I have a conda environment with pydeface and it's dependencies installed on it. But using your base conda environment while 
installing pydeface will work just fine but make sure to change/edit the code within the `pydeface-helper-notebook` according to 
your installation location. 

- **pydeface default facemask** The package uses a default facemask while defacing a scan. In some cases, like the Healthy Vounteers
dataset, the default facemask resulted in inaccurate defacing results. Inverting the default facemask and tweaking the regular
workflow produced more accurate defacing results. The decision to use the default facemask as is or not would depend on the dataset
in question. The helper notebook uses the modified workflow but it can also be used to run without any modifications with some 
edits to the code. The facemask used by default can be found within the package installation. In my case, it was 
`/home/arshithab/env/pydeface/lib/python3.7/site-packages/pydeface/data`
`<path/to/env/with/pydeface/installation>/lib/python3.7/site-packages/pydeface/data`
