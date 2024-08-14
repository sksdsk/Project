**General Information**
This project focuses on developing models for the Auto Flood Prediction University project, part of the course "Topics in Computer Science."

**Dataset Description**
Name:
SEN12-FLOOD: A SAR and Multispectral Dataset for Flood Detection

Publication Date:
September 18, 2020

Primary Repository:
Available at: IEEE Dataport

DOI:
https://dx.doi.org/10.21227/w6xz-s898

Version:
1.0

Description:
SEN12-FLOOD is a multimodal satellite image dataset (SAR + multispectral) designed for flood classification. It covers 337 locations, including cities and surrounding areas in West and Southeast Africa, the Middle East, and Australia, where flood events occurred between December 2018 and May 2019.

The dataset includes:

    Sentinel-2 Multispectral Images: Time series with 12 bands at a 10m ground-sampling distance, provided with Level 2A atmospheric correction.
    Sentinel-1 SAR Images: Time series provided with radiometric calibration and range doppler terrain correction using the SRTM digital elevation model. Each acquisition includes two raster images corresponding to the VV and VH polarimetry channels.
    Binary Labels: Time series of binary flood labels (flood or no flood) for each image/date.
File Name Structure:
All images are stored in raster format (GeoTIFF files).
Two json files, S1list.json and S2list.json are provided to describe respectively the Sentinel-1 and
Sentinel-2 images.The keys are the total number of images in the sequence, the folder name, the
geography of the observed area, and the description of each image in the series. The SAR images
description contains also the URLs to download the images. Each image is described by its
acquisition date, its label (FLOODING: boolean), a boolean (FULL-DATA-COVERAGE: boolean)
indicating if the area is fully or partially imaged, and the file prefix. For SAR images the orbit
(ASCENDING or DESCENDING) is also indicated.
Spatial Extent:
The observed areas correspond to 337 locations (cities and their surroundings ) in West and South-
East Africa, Middle-East, and Australia where a flood event occurred.
Temporal Extent:
The images and the flood labels correspond to the period going from 01/12/2018 to 31/05/2019.
Licence:
The dataset contains modified Copernicus data 2018-2019.
Copernicus Sentinel data are available under the Sentinel Terms and Conditions:
https://scihub.copernicus.eu/twiki/pub/SciHubWebPortal/TermsConditions/TC_Sentinel_Data_3107
2014.pdf
In particular, the User Rights article grant the User with Open-Access style permissions (use,
modification, sharing, publication and distribution).

**Project Description**
The project workflow includes:
    1) Data Preprocessing
    2) Feature Selection
    3) Model Training
    4) Model Evaluation
