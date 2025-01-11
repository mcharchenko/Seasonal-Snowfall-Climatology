# Seasonal Snowfall Climatology
This project uses the National Operational Hydrologic Remote Sensing Center's (NOHRSC) Snow Data Assimilation Snowfall Analysis (SNODAS) to create a high-resolution seasonal snowfall climatology of Western Washington.

The diverse topography of the Pacific Northwest produces many microclimates, creating notable differences in seasonal averages over short distances and elevation changes. These variations can be most noticeable through the western lowlands of the Pacific Northwest, especially across the Seattle, Portland, and Vancouver Canada metro areas, where population centers span from sea level to higher hills above 500-1000ft. The mild maritime winter climate of the western portion of the region generally keeps snow levels above the population centers, but occasional shots of colder air bring lower snow levels. What is frequently observed during these periods of lower snow levels is more snow and colder temperatures in the higher hills of the metro areas while the lower elevations see lower snow amounts, if any at all. Not to mention, larger topographical features frequently create mesoscale features such as convergence zones, which produce localized stationary bands of heavy precipitation which often contribute to highly variable snowfall totals.

Long term snowfall climatology from in-situ observations is limited in coverage through the Western US, and are mainly limited to lower elevation population centers. Therefore, average seasonal snowfall data in these population centers are rarely descriptive of seasonal snowfall amounts that are observed across the metro areas and their varying topography. The Snow Data Assimilation model uses remote sensing parameters and in-situ observations to create high resolution gridded data at a 1km x 1km resolution, which is enough to capture the rapidly changing topography across the lowlands. This model bridges a significant gap in observational data, and allows one to describe some of the nuanced snowfall climate zones across the region and thus draw conclusions to describe the snowfall climatology of the region. 

However, there are two primarily limitations to calling this a true climatology. First, the period of record only extends from 2008-Present, and this analysis only extends to the end of the 2024 season. True climatology records require a 30 year period od record, with the most recent period used being from 1991-2020. Second, while error correction is processed in the data assimilation model, some margins of error are still possible and may not be resolved due to the nature of data assimilation, which differs from in-situ observations that are frequently checked for sensor errors which can be resolved and calculated for due to the standardized nature of instrumentation. Therefore, this data output should only be used as a descriptor of snowfall climatology, and while comparison to in-situ snowfall climatology shows the output data to be accurate, its limitations desribed above should be noted during use-cases. 

## Repository Structure

- 'notebooks/access_SNODAS_data.ipynb': Access and download SNODAS snowfall data from the NOHRSC database.
- 'notebooks/process_and_map_SNODAS.ipynb': Process downloaded data and create snowfall climatology visualization.
- 'data/': Folder for storing SNODAS '.nc' files (not included in the repository).
- 'requirements.txt': Dependencies for the project.

## Setup Instructions
1. Clone this repository.
2. Install dependencies:
   '''bash
   pip install -r requirements.txt
