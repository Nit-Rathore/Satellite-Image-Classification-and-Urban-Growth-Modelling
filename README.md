# Satellite-Image-Classification
I trained an ANN model which classifies into four classes of  built-up, vegetation, barren lands and water bodies, using Landsat-5 data along with it's classified image 

We're using the classifier to generate Land Use/Land Cover(LULC) classification maps for different years. In this instance, I have used,
1997 multispectral image of Bangalore data to generate a LULC map for 1998. 
Another alterate method was tried where only a few samples are taken from 1997 to predict the entire classified image of the city in 1997.

# Urban Growth Modelling
Using the LULC maps, for various years, I built a Cellular automata model which predicts the built-up growth of the Delhi city in future years. 
It takes input as the classified image, along with population density maps, road network, slopes and restricted area maps and it
changes the cell value in the Matrix based on threshold values set.

# Results 
-As the spectral reflectance of the sun changes every year, we need to measure the devaitions before using it to predict the LULC maps.

-This approach of prediction works only when the season is same, when we build the classifier for summer season and try to predict for winter season,
the margin of error increases.

-Taking care of the above factors the exported classified image for 1998, gave a statistics of area-wise accuracy ~90% (Checked in Q-GIS)

-Classified Image of 1997 gave a statistics of area-wise accuracy of ~95% (Checked in Q-GIS)

-Urban Growth modelling accuracy for the actual image vs the predicted image was tried on a different years city and kappa coefficient was found to be 0.86


# Reqirements

1) gdal

2) tensorflow

3) Most of the related data can be found in usgs explorer website

# Future work
Feel free to use the code, and any future collaborations/suggestions to work on the project are always welcome.

