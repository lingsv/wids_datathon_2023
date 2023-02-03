Os dados abaixo são uma reprodução das explicações presentes na páginas do kaggle do Datathon WiDS.

## Aim

Your task is to predict the arithmetic mean of the maximum and minimum temperature over the next 14 days, for each location and start date.

You are provided with two datasets:

1.train_data.csv: the training dataset, where contest-tmp2m-14d__tmp2m, the arithmetic mean of the max and min observed temperature over the next 14 days for each location and start date, is provided
2.test_data.csv: the test dataset, where we withhold the true value of contest-tmp2m-14d__tmp2m for each row.

## Data Dictionary

Variable naming
Each variable name, prefix__suffix, consists of two parts (separated by a double underscore) that inform you of the meaning of the variable. The prefix indicates from which of the above-listed file the variable was derived (e.g. Madden-Julian oscillation, pressure, and potential evaporation from NOAA's surface_gauss etc), the suffix indicates the specific type of information that was extracted from the file.

Variable prefixes
contest-slp-14d: file containing sea level pressure (slp)

nmme0-tmp2m-34w: file containing most recent monthly NMME model forecasts for tmp2m (cancm30,
cancm40, ccsm30, ccsm40, cfsv20, gfdlflora0, gfdlflorb0, gfdl0, nasa0,
nmme0mean) and average forecast across those models (nmme0mean)

contest-pres-sfc-gauss-14d: pressure

mjo1d: MJO phase and amplitude

contest-pevpr-sfc-gauss-14d: potential evaporation

contest-wind-h850-14d: geopotential height at 850 millibars

contest-wind-h500-14d: geopotential height at 500 millibars
contest-wind-h100-14d: geopotential height at 100 millibars

contest-wind-h10-14d: geopotential height at 10 millibars

contest-wind-vwnd-925-14d: longitudinal wind at 925 millibars

contest-wind-vwnd-250-14d: longitudinal wind at 250 millibars
contest-wind-uwnd-250-14d: zonal wind at 250 millibars

contest-wind-uwnd-925-14d: zonal wind at 925 millibars

contest-rhum-sig995-14d: relative humidity

contest-prwtr-eatm-14d: precipitable water for entire atmosphere
nmme-prate-34w: weeks 3-4 weighted average of monthly NMME model forecasts for precipitation

nmme-prate-56w: weeks 5-6 weighted average of monthly NMME model forecasts for precipitation
nmme0-prate-56w: weeks 5-6 weighted average of most recent monthly NMME model forecasts for precipitation

nmme0-prate-34w: weeks 3-4 weighted average of most recent monthly NMME model forecasts for precipitation

nmme-tmp2m-34w: weeks 3-4 weighted average of most recent monthly NMME model forecasts for target label, contest-tmp2m-14d__tmp2m

nmme-tmp2m-56w: weeks 5-6 weighted average of monthly NMME model forecasts for target label, contest-tmp2m-14d__tmp2m

mei: MEI (mei), MEI rank (rank), and Niño Index Phase (nip)

elevation: elevation

contest-precip-14d: measured precipitation

climateregions: Köppen-Geigerclimateclassifications

Variables without prefix
Some variables do not have a prefix. Instead, each variable name in its entirely indicates the information the variable captures.

lat: latitude of location (anonymized)
lon: longitude of location (anonymized)
startdate: startdate of the 14 day period
sst: sea surface temperature
icec: sea ice concentration
cancm30, cancm40, ccsm30, ccsm40, cfsv20, gfdlflora0, gfdlflorb0, gfdl0, nasa0, nmme0mean: most recent forecasts from weather models
Target
contest-tmp2m-14d__tmp2m: the arithmetic mean of the max and min observed temperature over the next 14 days for each location and start date, computed as (measured max temperature + measured mini temperature) / 2
