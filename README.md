# Spatial Assessment of Trace Element Bioavailability in Headwater Streams

**Last updated:** 4/22/2026  
**Developed by:** Cecilia Albert-Black  
**Project:** Watershed Dynamics Evolution (WaDE) Science Focus Area at Oak Ridge National Lab (ORNL), in collaboration with a Powell Center Working Group funded by the United States Geological Survey (USGS)  
**Dataset:** WaDE Synoptic Survey Dataset collected bi-monthly (Jun. 2023 – Feb. 2025) from sites in the East Fork Poplar Creek Watershed (Oak Ridge, TN)

---

## Workflow

### WaDE Dataset Cleaning
The first step in this workflow was to clean the WaDE Synoptic Survey Dataset by selecting variables of interest for BLM and filtering by detection limits using an Rmd file.

### Zinc or Copper Folders
*(Zinc folder should be run before Copper)*

#### 1. Running BLM
- **Inputs:** BLM data entry Excel file created via R Markdown  
- **Process:** Copied into desktop BLM and executed  
- **Outputs:** Saved BLM output files  

#### 2. Dataset Merging
- Merging WaDE Synoptic Survey dataset with BLM outputs to create the raw `Bioavailability_Master_Spreadsheet.xlsx`

#### 3. Dataset Cleaning
- Unit conversions and new variable creation stored in `Bioavailability_Master_Spreadsheet_Clean.xlsx`

#### 4. Exploratory Data Analysis
- EDA of variables stored in Excel files
- log transformed variables stored in `Bioavailability_Master_Spreadsheet_Clean2.xlsx`

#### 5. Cluster Analysis
- Sample-level clustering → `Typology`  
- Site-level clustering → `Typology2`  
- Both stored in `Bioavailability_Master_Spreadsheet_Clean3.xlsx`

#### 6. Statistical Analysis
- Uses  `Bioavailability_Master_Spreadsheet_Clean3.xlsx`
- All statistical tests + outputs stored in Excel files + plot images

#### 7. Sensitivity Analyses
Each analysis with outputs stored in subfolders with Excel + plots images
- **Carbonate system assumptions**  
- **Humic acid system assumptions**

