# geotechdata
Exploration of publicly available Geotechnical Investigation Data

## Notebook 0 - Download and Pre-process data
Downloading and processing geotechnical investigation data from Norways Database of Geotechnical Investigations (NADAG) 

## Notebook 1 - Interpreting u0 (in-situ pore pressure) from CPT data
Experimenting with interpreting u0 based on measured u2 in CPTu data.
Establishd a baseline results that estimate u0 based on assuming the groundwater table is 2 m below the start of the CPT, an analytical method to fit a curve, and a XGBoost based method.

Using an XGBoost model (trained on a dataset from Premstaller) to predict u0 results with a RMSE of 8 kPa on the NADAG dataset  - which is an improvement both on the constant depth assumption and my analytical method.
![image](https://github.com/lucasfabbri/geotechdata/assets/25036638/b5c6be33-c3c1-4fb2-a82d-e33f08fa2b95)
![image](https://github.com/lucasfabbri/geotechdata/assets/25036638/977a235b-5636-40cf-a0c3-81d36ebb9410)
Median error: 7.93 Average error: 12.52 Max error: 114.68

## Notebook 2 - Exploring correlations in laboratory, total sounding, and CPT data 
Exploring how the dataset compares with existing classification and correlation schemes.

### Examples:
Robertson (2009) updated non-normalized SBT vs Visual Description Classification 
1370 total visual descriptions reported as representative of 1577.4 m of CPT data (1310 used in plot)

![image](https://github.com/lucasfabbri/geotechdata/assets/25036638/4e655c69-2c04-4189-9482-99060186ee94)



Robertson et al. (1986) non-normalized SBT vs Grain Size Features
256 total grain size distributions reported as representative of 183.1 m of CPT data

![image](https://github.com/lucasfabbri/geotechdata/assets/25036638/a78521cf-8c3e-492e-9c65-a4247cb0cd1e)


Haugen et al. (2016) Total Sounding Classification System and  Visual Description Classification
![image](https://github.com/lucasfabbri/geotechdata/assets/25036638/0e4c4996-9d53-4322-bdf4-7d4a8c059545)

## Notebook 3 - Exploring what data is present in the various Quick Clay Hazard Zones

![image](https://github.com/lucasfabbri/geotechdata/assets/25036638/35a17544-8b35-4b46-b74d-41482119aa09)

![image](https://github.com/lucasfabbri/geotechdata/assets/25036638/a5a17e0d-9835-4184-af7b-670f7265c06e)


