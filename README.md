# Rhode Island Election Shapefile

This shapefile was processed by Professor Ellen Veomett and her student Ananya Agarwal.

# **Sources**

Obtain the following data from Restricting Data Hub

[Population data](https://redistrictingdatahub.org/dataset/rhode-island-block-pl-94171-2020-by-table/): based on the decennial census at the Census Block level on 2020 Census Redistricting Data

[Congressional District data](https://redistrictingdatahub.org/dataset/2022-rhode-island-congressional-districts-approved-plan/): 2022 Rhode Island Congressional Districts plan enacted on 2/7/22

[State House District data](https://redistrictingdatahub.org/dataset/2022-rhode-island-house-of-representatives-districts-approved-plan/): 2022 State House Approved Plan

[State Senate District data](https://redistrictingdatahub.org/dataset/2022-rhode-island-state-senate-districts-approved-plan/): 2022 State Senate Approved Plan

[2020 election data](https://redistrictingdatahub.org/dataset/vest-2020-rhode-island-precinct-and-election-results/)**:**  VEST 2020 Rhode Island precinct and election results

[2018 election data](https://redistrictingdatahub.org/dataset/vest-2018-rhode-island-precinct-and-election-results/)**:**  VEST 2018 Rhode Island precinct and election results

[2016 election data](https://redistrictingdatahub.org/dataset/vest-2016-rhode-island-precinct-and-election-results/)**:**  VEST 2016 Rhode Island precinct and election results

# **Processing**

Demographic data were aggregated from the census block level and precincts were assigned to districts using [MGGG's proration software](https://github.com/mggg/maup). Election data were also prorated onto VTDs from the original precinct shapefile using the `maup` package.

# **Metadata**

Below is a brief description of each of the listed variables in the attribute table of the VTD shapefile:

- `STATEFP`: State FIPS code
- `COUNTYFP`: County FIPS code
- `VTDST20`: Voting tabulation district FIPS code
- `GEOID20`: Geographical ID
- `NAME20`: Voting tabulation district name
* `Shape__Are`: Precinct area in square degree
* `Shape__Len`: Precinct perimeter in degree
* `JOINID`: Precinct ID
* `PRENAME`: Precinct name 
* `REGVOT16`: Number of registered voters for 2016 general election
* `TOTVOT16`: Number of ballots cast in 2016 general election
* `PRES16D`: Number of votes for 2016 Democratic presidential candidate
* `PRES16R`: Number of votes for 2016 Republican presidential candidate
* `REGVOT18`: Number of registered voters for 2018 general election
* `TOTVOT18`: Number of ballots cast in 2018 general election
* `GOV18D`: Number of votes for 2018 Democratic gubernatorial candidate
* `GOV18R`: Number of votes for 2018 Republican gubernatorial candidate
* `SEN18D`: Number of votes for 2018 Democratic senate candidate
* `SEN18R`: Number of votes for 2018 Republican senate candidate
* `TOTPOP`: Total population 
* `NH_WHITE`: White, non-hispanic, population
* `NH_BLACK`: Black, non-hispanic, population
* `NH_AMIN`: American Indian and Alaska Native, non-hispanic, population
* `NH_ASIAN`: Asian, non-hispanic, population
* `NH_NHPI`: Native Hawaiian and Pacific Islander, non-hispanic, population
* `NH_OTHER`: Other race, non-hispanic, population
* `NH_2MORE`: Two or more races, non-hispanic, population
* `HISP`: Hispanic population
* `VAP`: Total voting age population
* `HVAP`: Hispanic voting age population
* `WVAP`: White, non-hispanic, voting age population
* `BVAP`: Black, non-hispanic, voting age population
* `AMINVAP`: American Indian and Alaska Native, non-hispanic, voting age population
* `ASIANVAP`: Asian, non-hispanic, voting age population
* `NHPIVAP`: Native Hawaiian and Pacific Islander, non-hispanic, voting age population
* `OTHERVAP`: Other race, non-hispanic, voting age population
* `2MOREVAP`: Two or more races, non-hispanic, voting age population
* `HDIST`: State house district ID
* `SENDIST`: State senate district ID
* `CD`: Congressional district ID

# **Projection**

The shapefile uses a UTM NAD83 projection (EPSG: 4269).