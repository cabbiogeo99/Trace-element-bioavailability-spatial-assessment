# Spatial Assessment of Trace Element Bioavailability in Headwater Streams
### Last updated: 4/1/2026
### Developed by Cecilia Albert-Black
### Project: Watershed Dynamics Evolution (WaDE) Science Focus Area at Oak Ridge National Lab (ORNL) and in collaboration with a Powell Center Working Group, funded by the United States Geological Survey (USGS)
### Dataset: WaDE Synoptic Survey Dataset collected bi-monthly during Jun. 2023 – Feb. 2025 from several sites within the East Fork Poplar Creek Watershed in Oak Ridge, TN

### Workflow
## WaDE Dataset Cleaning folder
The first step in this workflow was to clean the WaDE Synoptic Survey Dataset by selecting the variables of interest to run in BLM and filtering out by detection limits using the Rmd file.

## Zinc or Copper folders (Zinc folder is intended to be run first before Copper folder files)
# 1. Running BLM folder
Data inputs: Here a BLM data entry excel file was created using the R markdown file. The contents of the excel file were copied, pasted into, and ran in BLM (desktop version).
Data outputs: The BLM output files were saved in this folder.

# 2. Dataset merging folder
Merging of variables from the WaDE Synoptic Survey Dataset and BLM output files to create a raw Bioavailability Master Spreadsheet was conducted using the Rmd file.

# 3. Dataset cleaning folder
Here, unit conversions of variables and creation of new variables were performed from the Bioavailability Master Spreadsheet to create the clean version of the Bioavailability Master Spreadsheet.

# 4. Exploratory data analysis folder
Exploratory data analysis of samples and site characteristics was performed in this folder. Log-transformed variables were added to the Bioavailability Master Spreadsheet to create a 2nd clean version.

# 5. Cluster analysis
K-means cluster analysis of BLM predictor variables following 2 methods: 
- Sample-level clustering: produces Typology variable
- Site-level clustering: produces Typology2 variable
Both clustering assignments (Typology and Typology2) are saved within the final excel file called Bioavailability_Master_Spreadsheet_Clean3.xlsx.

# 6. Statistical analysis folder
All statistical analyses were performed in this folder and the results are saved in excel files and plots within sub-folders.

# 7. Sensitivity analyses folder
Two sensitivity analyses were performed in this folder, whose output is contained in excel files and plots within sub-folders.

