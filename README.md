# Satellite-Image-Classification
Using Landsat-5 data along with it's classified image, I trained an ANN model which classifies into four classes of built-up, vegetation, barren lands
and water bodies.  
We are using this classifier to generate Land Use/Land Cover(LULC) classification maps for different years. In this instance, I have used,
1997 multispectral image of Bangalore data to generate a LULC map for 1998. 
Another alterate method was tried where only a few samples are taken from 1997 to predict the entire classified image of the city in 1997.

# Urban Growth Modelling
Using the LULC maps, for various years, I built a Cellular automata model which predicts the built-up growth of the city in future years. 
It takes input as the classified image, along with population density maps, road network, slopes and restricted area maps and it
changes the cell value in the Matrix based on threshold values set.

# Results 
-As the spectral reflectance of the sun changes every year, we need to measure the devaitions before using it to predict the LULC maps.
-This approach of prediction works only when the season is same, when we build the classifier for summer season and try to predict for winter season,
the margin of error increases.
-Taking care of the above factors the classified image for 1998, gave an area wise accuracy of 90.2% (Checked in Q-GIS)
-Classified Image of 1997 gave an area wise accuracy of ~95% (Checked in Q-GIS)


# Reqirements

1) gdal

2) tensorflow

3) Most of the related data can be found in usgs explorer website

# Future work
Feel free to use the code, and any future collaborations to work on the project are welcome.

