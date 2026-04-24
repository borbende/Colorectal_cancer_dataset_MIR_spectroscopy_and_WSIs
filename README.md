# Colorectal cancer dataset MIR spectroscopy and WSIs

## Description

This is a small supplementary repository to support the handling of the Multimodal colorectal cancer dataset (FT-IR spectroscopy and Whole Slide Imaging) available on Zenodo [10.5281/zenodo.17790337](https://doi.org/10.5281/zenodo.17790337). The dataset contains data recorded from colorectal cancerous tissue samples collected from 130 patients. 9 tissue microarrays (TMA) were included in the dataset, meaning 9 Whole Slide Images and many tissue core-wise mid-infrared (MIR) measurements made up the entire dataset. Further details can be viewed in the description of the Zenodo dataset.


```bash 
notebooks
├── CRC_data_showcase.ipynb
├── CRC_metadata_val.ipynb
├── MIR_technval.ipynb
├── WSI_technval.ipynb
├── MIR_fsm_to_txt.ipynb
├── MIR_preprocessing.ipynb
```

- <strong>MIR_fsm_to_txt.ipynb</strong>: a function that uses the specio Python package to load .fsm files and then converts them into .txt tables and generates the spatial positions of the mid-infrared spectra, while also saving the spectral metadata to a .json file.
- <strong>CRC_data_showcase.ipynb</strong>: an example notebook for looking at the different data types in the database.
- <strong>CRC_metadata_val.ipynb</strong>: a notebook containing some basic analysis on the main metadata files.
- <strong>WSI_technval.ipynb</strong>: the technical validation workflow of the Whole Slide Images using OpenSlide Python complete with tissue core-wise sharpness computation and circle detection.
- <strong>MIR_technval.ipynb</strong>: the technical validation workflow of the mid-infrared spectroscopy dataset and some data analysis tools: conversion from transmittance to absorbance, filtering out background spectra, signal-to-noise ratio distributions, the presence of atmospheric effects, and baseline drift.
- <strong>MIR_preprocessing.ipynb</strong>: the preprocessing pipeline complete with background filtering, a small PCA-based outlier detection method, baseline correction and atmospheric correction.

## Data availability
The mentioned dataset is available in the following Zenodo repository: Borkovits, B. et al. Multimodal colorectal cancer dataset (FT-IR spectroscopy and Whole Slide Imaging). Zenodo. [10.5281/zenodo.17790337](https://doi.org/10.5281/zenodo.17790337) (2025).

## Citation

Please cite one of the articles in the next section.

## Related articles
These already published articles processed a small part of the dataset.
1. Borkovits B, Kontsek E, Pesti A, et al. Classification of colorectal primer carcinoma from normal colon with mid-infrared spectra. Journal of Chemometrics. 2024; 38(7):e3542. [doi:10.1002/cem.3542](https://doi.org/10.1002/cem.3542)
2. Borkovits, B., Török, C., Kontsek, E. et al. Fourier transform mid-infrared imaging and rapid evaporative ionization mass spectrometry imaging in FFPE colorectal adenocarcinoma samples. Pathologie (2025). [https://doi.org/10.1007/s00292-025-01502-1](https://doi.org/10.1007/s00292-025-01502-1)

