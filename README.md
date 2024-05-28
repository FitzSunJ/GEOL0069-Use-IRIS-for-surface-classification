# GEOL0069: Surface Classification Using IRIS

This project aims to utilize IRIS to generate training data for a wide range of applications in surface classification. The primary objective is to classify different types of land cover and land use using remote sensing data obtained from Sentinel-2 satellite imagery.

## Project Overview

Surface classification is a crucial task in Earth observation, helping in various applications such as environmental monitoring, urban planning, and agricultural management. This project leverages the power of IRIS (Intelligently Reinforced Image Segmentation) to accurately classify and label surface types from satellite images.

## Methodology

### Data Collection

- **Data Source**: Sentinel-2 satellite imagery.
- **Tools Used**: Google Earth Engine (GEE), Python, and IRIS.

### Steps Involved

1. **Data Fetching**: Utilize Google Earth Engine to fetch satellite imagery.
2. **Preprocessing**: Clean and preprocess the data to make it suitable for analysis.
3. **Segmentation**: Use IRIS to segment the satellite images into different surface types.
4. **Classification**: Apply machine learning algorithms to classify the segmented regions.
5. **Validation**: Validate the classification results using ground truth data.

This project focuses on the best use of IRIS to generate training data for a wide range of applications.
I choose use Docker to deploy IRIS. First, build an image (run from IRIS's root directory). Then, you can use docker run to launch IRIS. However, please note that port-forwarding is needed (here we use port 80 as an example for a typical http setup, but the port number can be set in your IRIS config file) and the directory to your project also needs to be given as a volume to docker.
docker pull totony4real/iris:1.0
