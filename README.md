# spectral-dataset-RockSL
[license](https://creativecommons.org/licenses/by/4.0/ "悬停显示文字")

an integrated open mineral spectral library from shared libraries (USGS,JHU,JPL,ASU,MISA, etc.) and measurement spectra in our own laboratory. We hope that more researchers will join to improve the availability and practical value of RockSL for remote sensing community. 

## Data source
| Spectral Library     | Wavelength range    | Particle size    | Shared Format  | Data resource |
| ---------- | :-----------:  | :-----------: | :-----------:  | :-----------: |
| USGS      | 0.2-200μm    | μm level    | ASCII  |  https://www.usgs.gov/labs/spec-lab/capabilities/spectral-library  |
| JPL     | 0.4-2.5μm    | <45μm，45-125μm,125-500μm| ASCII  | http://speclib.jpl.nasa.gov |
| JHU     | 0.4-14μm; 2.08-25μm| μm level    | ASCII  | http://speclib.jpl.nasa.gov |
| PDS     | 0.3-26.0μm    | μm level    | ASCII  | https://speclib.rsl.wustl.edu/search.aspx  |
| ASU     | 5.0-45μm    | 710-1000μm    | ASCII/HDF  |  https://speclib.asu.edu/  |
| MISA    | 0.25-5.0μm    | /   | Image  |  http://www.organchem.csdb.cn/scdb/  |
| CSU Lab     | 0.3-14μm    | μm level    | ASCII/CSV  | https://github.com/CSU-PCP-XBS/spectral-dataset-RockSL |

## Database structure
The data structure of RockSL (shown in Figure 1) contained several relational data tables mainly used to save reference spectral data with related parameters, attribute data, classification code of rocks and minerals, and the specific information of spectrometers. The relational table of rock/mineral code as the main relational table was designed to store sematic and classification contents for data consolidation from diverse regions, and to facilitate rapid retrieval. The relational table of mineral/rock code and mineral/rock type records the classification information. The table of mineral/rock attribute records the physical and chemical properties, while spectral data information records spectral data and related metadata. The table of instrument information records the spectrometer information. The numbers (i.e., 1 and m) represent the number of records in each table, indicating that one record in the table (e.g., code of mineral/rock type) corresponds to multiple records in another table (e.g., code of mineral/rock).

![image](https://user-images.githubusercontent.com/66400818/147445088-f581487e-c860-418e-bb37-fc73a0a52e05.png)

## Spectral data description


## Recommended citation
Xie, B., Zhou, S., Wu, L., Mao, W., Wang, W., 2021. RockSL: an integrated rock spectral library for better global shared services(accepted), Big Earth Data, DOI: https://doi.org/10.1080/20964471.2021.2017111

## RockSL database management


## Data policy
This work is mainly to unify the format and semantics of spectral data of each shared spectral library and tested data. If there exists the problem with  quality of shared data , please contact original developers or visit related website. Besides, if the RockSL is cited in your scientific research projects or papers, please pay attention to cite the relevant works of shared database creators (you can get in touch with me or go to the corresponding official website).
**USGS**

**JPL/JHU**
The ECOSTRESS spectral library includes data from three other spectral libraries: Johns Hopkins University (JHU)、Jet Propulsion Laboratory (JPL) and United States Geological Survey (USGS - Reston). If you use data from the ECOSTRESS spectral library in a publication we ask that you reference the following articles: 
* Meerdink, S. K., Hook, S. J., Roberts, D. A., & Abbott, E. A. (2019). The ECOSTRESS spectral library version 1.0. Remote Sensing of Environment, 230(111196), 1–8. 
* Baldridge, A. M., S.J. Hook, C.I. Grove and G. Rivera, 2009.The ASTER Spectral Library Version 2.0. Remote Sensing of Environment, vol 113, pp. 711-715.

**ASU**

**PDS**

**MISA**



## Disclaimer
All data in this repository was collected/calculated/calibrated from multiple publicly available data sources that do not always agree. While we'll try our best to keep the information up to correct, we make no representations or warranties of any kind, express or implied, about the completeness, accuracy, reliability, with respect to the data. We do not bear any legal responsibility for any consequence caused by the usage of data provided. Reliance on the data for use of the data in commerce is strictly prohibited. 

## Prospects
1. We will upload and collect more relevant open source and test spectrum data and update them later, 
2. We will upload the database management software of the RockSL (this dataset is built based on SQL server and would be distributed in SQLite).
3. we will establish the website for mineral/rock spectral data interchange.
