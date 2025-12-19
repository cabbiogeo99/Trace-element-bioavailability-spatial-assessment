This repository was developed by Cecilia Albert-Black and is still "under construction" for the Spatial Assessment of Bioavailability Across Headwater Streams Project within the Watershed Dynamics Evolution (WaDE) Science Focus Area at Oak Ridge National Lab (ORNL) and in collaboration with a Powell Center Working Group, funded by the USGS.

This repo contains all steps followed by Cecilia used to run BLM from data contained in the WaDE Synoptic Survey Campaign conduced from Jun. 2023 – Feb. 2025 by obtaining bi-monthly samples from the East Fork Poplar Creek Watershed in Oak Ridge, TN.

This repo is meant to be followed using the folders in numeric order to conduct each step:

1. Running BLM folder
	- Data inputs sub-folder: develop input files from the WaDE_Synoptic_Summary.xlsx dataset to run Zn-BLM and Cu-BLM (both in speciation and toxicity mode) under the following conditions: 
		i. HA 10% Closed System (default)
		ii. HA 10% Open System (no DIC input variable)
		iii. HA 80% Closed System (higher humic acid content)
	- Data outputs sub-folder: all BLM output files (both in speciation and toxicity mode) under each condition.

2. Dataset merging folder: merging the WaDE_Synoptic_Summary.xlsx with relevant variables from the BLM output files to create the Bioavailability_Master_Spreadsheet.xlsx with conditions separated by tab.

3. Dataset cleaning folder: cleaning variables by standardizing concentration variables, creating total bioavailable element and relative proportion of bioavailable element, and creating categorical variables from numeric ones (development, distance from main stem, drainage area, and relative elevation).

4. Exploratory data analysis folder: contains sub-folders for each condition which contains code to explore the distribution of variables under each condition.

5. Statistical data analysis: contains all data analysis including typological classification (clustering), multiple linear regression, Kruskal-Walis tests, and graphing for data under the default condition (HA 10% Closed System). Sub-folders contain all plots and visual outputs from the Rmd file.

6. Sensitivity analyses (***to be developed***): contains sensitivity analyses comparing the results from the default condition with that of the other two conditions to determine whether our DIC measurements contained a significant amount of error as to influence the results and to assess whether a higher percentage of DOC humic acid content significantly changes the results from the baseline condition.

