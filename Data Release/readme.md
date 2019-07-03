This folder contains source data, processing codes (in the form of Jupyter Notebooks), and a cache of processed data for a data release of information associated with WLCI species. 

# Species and Capability Source Information
As a starting point for this work, we built a list of species that were mentioned in WLCI work using xDD processes explained in the notebook wlci-species/build-specie-list.ipynb 

# Processing Logic
The building of this dataset is based in a set of logical processes we are building for a variety of work on a platform called the Biogeographic Information System. The codes that consult other data sources and assemble information for use in this data release come from a Python package called [bispy](https://github.com/usgs-bcb/bispy). The particular workflows described and executed here can be operated in a variety of ways from producing something like the local cache of data we include in this data release to running operationally on a cloud system, checking sources and building data continuously.

# Workflow
Some of the steps in this system build upon each other while others can be operated independently. The primary initial step for most processes involves reading out the list of species, assembling species names and available identifiers for use in other steps.