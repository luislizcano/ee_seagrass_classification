# Semi-Automated Seagrass Classification Using Earth Engine Python API
[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fluislizcano%2Fee_seagrass_classification&count_bg=%23969696&title_bg=%23FFD812&icon=github.svg&icon_color=%23E7E7E7&title=Visits&edge_flat=false)](https://hits.seeyoufarm.com)
[![GPL license](https://img.shields.io/badge/License-GPL-blue.svg)](http://perso.crans.org/besson/LICENSE.html)

**Description:** This script classify dense seagrass beds in satellite images (from Sentinel and Landsat sensors) using machine learning (Support Vector Machine). The outputs can be exported to EE Assets. All the training and validation matrices and accuracies can be saved as an Excel file in your working directory.<br/>

**NOTE:** The classifications will use only the aerosol (if available), blue, green, red and Blue/Green (from Depth Invariant Index) bands.<br/>

By Luis Lizcano-Sandoval<br/>
College of Marine Science, University of South Florida<br/>
luislizcanos@usf.edu<br/>
Updated: 09/03/2021<br/>

## **Workflow:**

1. Import required images, collections, data, etc.
2. Mask clouds, land, and deep areas >20m
3. Apply Depth-Invariant Index (band-ratios)
4. Sample bands: B1, B2, B3, B4, B/G
5. Train models and classify (SVM)
6. Get confusion matrices and accuracies
7. Export output to EE Assets (.tiff)
8. Save matrices in local computer (.xlxs)

## Demo:

### Sentinel-2 L2A Image:
<img src="https://raw.github.com/luislizcano/ee_seagrass_classification/main/img/img-sentinel2.png" width="800">

### Cloud Mask:
<img src="https://raw.github.com/luislizcano/ee_seagrass_classification/main/img/img-cloud-mask.png" width="800">

### Land Mask:
<img src="https://raw.github.com/luislizcano/ee_seagrass_classification/main/img/img-land-mask.png" width="800">

### Depth Mask:
<img src="https://raw.github.com/luislizcano/ee_seagrass_classification/main/img/img-depth-mask.png" width="800">

### Classified Image:
<img src="https://raw.github.com/luislizcano/ee_seagrass_classification/main/img/img-classified.png" width="800">
