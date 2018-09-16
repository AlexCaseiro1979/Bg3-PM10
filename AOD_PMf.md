---
title: A boundary condition model for particulate matter concentrations based on MODIS observations`
author: Alexandre Caseiro
output: pdf_document
---
# ideas
develop a system to produce background pollutant concentrations using satellite products.
example: MODIS L3 AOD product (1 month average at the 1 degree spatial resolution) could be used to estimate PM background values.

# motivation
when working in the industry, we often had the limitation that we did not know about background levels in some countries where there is no monitoring network (e.g. in Africa).
Background concentrations are a fundamental boundary condition for modelling works.
In the academic world, there is MOZART, which is based on a model.
The idea of this work is to develop something based on observations, that would be a complement to MOZART.

# workflow
The basic idea is to calibrate the AOD product with concentrations measured at background sites.
1. get the data from background sites, e.g. for Europe that should be easy. The more data, the better.
2. get the MODIS L3 AOD product, that s also easy.
3. correlate the PM concentrations at the background site (monthly averages) to the AOD of the prduct pixel covering that station.
From previous work, I know that the model will perform poorly, but that its performance will increase when bringing in non-linearity and ancilliary data, such as relative humidity, temperature, ...
4. validate against MOZART and against some sites that would not be used to create the model.

