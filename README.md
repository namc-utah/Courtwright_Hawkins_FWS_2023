# Courtwright_Hawkins_FWS_2023
Data associated with the Courtwright Hawkins 2023 Freshwater Science publication

This repository contains the following files:

* final_indices.csv which contains the 16 indices compared in the paper for reference and degraded sites. Basic sample information such as sampleDate, NHD unique identifier (COMID), and latitude and longitude is also provided.
* CA_validation_results.csv which contains the mIR and CSCI comparisons at a set of independent California sites that were used in the publication as a validation dataset.
	
Predictors
* predictors.csv which contains the final predictors used in the final indicies, most of these come directly from EPA's StreamCat dataset and use the StreamCat naming convention. Any other predictors use naming conventions described in the Supplimental material. Exceptions are pct_46003 and length_46006, which are referred to as %NP25km and P25km in the publication respectively.
* Merritt_et_al_2021_predictions folder contains csvs named by USGS 2 digit HUC. Each csv contains predictions of reference flow regime components by NHD unique identifier (COMID) based on methods in Merritt et al. 2021 Water publication.

OE
* OE_trad_predictive_model_scripts_v4.2.1 John VanSickle's scripts for creating traditional RIVPAC O/E indicies. This folder contains its own README file.
* macroinvert_presence_absence.csv which contains a site by species presence/absence matrix for reference and degraded sites.
* OE_rra_nf_calculation.xlsx is a series of worksheets that calculate the trait-based O/E using the equation presented in the publication. Only example calculations for O/E-rra without novel measures of flow regime are provided.
* Two R workspaces that contain randomforest objects needed to run the two versions of the traditional taxa-based O/E: nf (without novel measures of flow regime.

MMI_IndividualMetrics
* macroinvert_metrics.csv which contains all metrics considered in MMI development for reference and degraded sites.
* MetricRandomForestModels.Rdata which contains all randomforest model objects needed to calculate the final mMMIs and modeled richness metrics.
