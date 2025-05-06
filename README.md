# Census 2010 to 2020 Geographies

Takes in a finalized tract dataset and standardizes the values to fit 2020 tract boundaries. assumes that the dataset fits the data commons conventions for finalized data (columns: geoid, year, measure, value, moe, region_type || measure names: snake case - underscore delimeter) param: data(dataframe) -> tract data fitting data commons conventions (outlined above) param: filter_geo(character - default="state") -> geographic level to keep consistent with original data. (for example, if your original data only contains specific states like Virginia, use "state". if your original data only contains specific counties like Fairfax and Arlington, use "county") return: same dataframe with values standardized to 2020 boundaries

## Installation
remotes::install_github("https://github.com/uva-bi-sdad/sdc.census10to20")
