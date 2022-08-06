# Satellite-Image-Classification
Using Landsat-5 data along with it's classified image, I trained an ANN model which classifies into four classes of built-up, vegetation, barren lands
and water bodies.  
We are using this classifier to generate Land Use/Land Cover(LULC) classification maps for different years. In this instance, I have used,
2013 satellite image of Bangalore data to generate a LULC map for 2011 and 2014

# Urban Growth Modelling
Using the LULC maps, for various years, I built a Cellular automata model which predicts the growth of the city in future years. 
It takes input as the classified image, along with population density maps, road network, slopes and restricted area maps and it
changes the cell value in the Matrix based on threshold values set.

# Results
Based on comparision, we used the 2009 data to predict land cover with 2014 and then compared with actual 2014 data in GRASS GIS to compare maps by, area in hectares 
and % land cover, accuracy upto 96% was achieved.

# Reqirements

1) gdal

2) tensorflow

3) Most of the related data can be found in usgs explorer website

# Future work
Feel free to use the code, and any future collaborations to work on the project are welcome.

