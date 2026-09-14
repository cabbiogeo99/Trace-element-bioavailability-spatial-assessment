# Trace Metal Bioavailability Varies with Flow Regime and Land Cover in a Headwater Stream Network

**Last updated:** Sept, 2026  
**Developed by:** Cecilia Albert Black  
**Funding/Project:** Watershed Dynamics Evolution (WaDE) Science Focus Area at Oak Ridge National Lab (ORNL), in collaboration with a Powell Center Working Group funded by the United States Geological Survey (USGS)  
**Dataset:** WaDE Synoptic Survey Dataset collected bi-monthly (Jun. 2023 – Feb. 2025) from sites in the East Fork Poplar Creek Watershed (Oak Ridge, TN)

---

## Workflow

### WaDE Dataset Cleaning
The first step in this workflow was to clean the WaDE Synoptic Survey Dataset by selecting variables of interest for BLM and filtering by detection limits using an Rmd file.

### Zinc or Copper Folders
*(Zinc folder should be run before Copper)*

#### 1. Running BLM
- **Inputs:** BLM data entry Excel files created in R 
- **Process:** Copied and pasted into desktop BLM and executed  
- **Outputs:** Saved BLM output files  

#### 2. Dataset Merging
- Merging WaDE Synoptic Survey dataset with BLM outputs to create the raw `Bioavailability_Master_Spreadsheet.xlsx`

#### 3. Dataset Cleaning
- Unit conversions and new variable creation stored in `Bioavailability_Master_Spreadsheet_Clean.xlsx`

#### 4. Exploratory Data Analysis
- Exploratory data analysis of BLM input and output variables stored as Excel files
- log transformed variables stored in the updated `Bioavailability_Master_Spreadsheet_Clean2.xlsx`

#### 5. Cluster Analysis (only in Zn folder)
- Sample-level clustering → `Typology`  
- Site-level clustering → `Typology2`  
- Both cluster-method typologies stored in `Bioavailability_Master_Spreadsheet_Clean3.xlsx`

#### 6. Statistical Analysis (separate for Zn and Cu output data, given BLM can only consider bioavailability of 1 metal at a time)
- Uses `Bioavailability_Master_Spreadsheet_Clean3.xlsx` to conduct statistical tests
- Outputs stored in Excel files and plots as images

#### 7. Sensitivity Analyses
Each analysis with outputs stored in subfolders with Excel + plots images
- **Carbonate system assumptions** Closed vs. open-system
- **Humic acid system assumptions** Range from 10-60%

