# Planned revisions to reproduction of Malcomb et al (2014)

## Author: Colman Bashore


## Modifications
I plan to modify this reproduction study through calculating an average vulnerability score for each traditional authority.
Figure 5 of the original study and reproduction presents the final results of the vulnerability model in a raster grid. 
While this is helpful for seeing the general patterns of vulnerability across the nation, the raster model is quite grainy and difficult to interpret. 
My modification is to calculate a zonal statistic for each traditional authority of the mean of vulnerability. 
Essentially, my code will take the mean of each pixel in the vulnerability raster layer for a given traditional authority and save that as the vulnerability score for that traditional authority. 
This will allow the user to get a better sense of the trends of vulnerability on a more applicable scale than small gridded pixels. 

## Visualization and comparison of results

The result of my modification should be a new polygon layer with the same geometry as the traditional authorities but an added field that represents the average vulnerability score in that geometry. 
I will be able to visualize this modification by plotting the new polygon layer using tmap. 
The map will be a cloropleth that shows which TA's have higher vulnerabilities than others according to our model.
It can be compared to the original figure 5 which also visualizes vulnerability but on a raster grid. 
The modification will have been successful if the new map is more visually clear and also provides a useful unit of measurement of vulnerability for applying funding efforts. 



