### Overview ###
This folder contains scripts and outputs for clustering analyses of bioavailability data using Biotic Ligand Model (BLM) input variables. Two clustering approaches are implemented:

Clustering by individual samples
Clustering by site-averaged BLM variables

These approaches produce two classification variables:

Typology → sample-level clustering
Typology2 → site-level clustering

### Workflow (Run in Order) ###

# Step 1
Run sample-level clustering file: Clustering_by_Sample.Rmd
# Output: 
Bioavailability_Master_Spreadsheet_Clean3.xlsx (version _Clean2 with Typology column)
Plots in folder called Identifying Typology Plots

# Step 2
Add site-level clustering by running site-level clustering file: Clustering_by_Site.Rmd
# Output: 
Bioavailability_Master_Spreadsheet_Clean3.xlsx (updated with Typology2 column)
Plots in folder called Identifying Typology2 Plots
