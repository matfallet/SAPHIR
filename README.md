# Image Explorer

### Introduction 

### Requirements 
#### Images 
The image file to analyse must be in TIFF format. It can be up to 4 dimensions with third and fourth dimensions representing channel and depth (z coordinate). 

#### DataFiles & ROIs
The other necessary files are : results.csv, intensity.txt and RoiSet.zip. These files must be in a repository in the same location as the image, this repository must be named "'filename of the image.tif'_out". 

##### File intensity.txt 
File containing for each ROI its ID and its intensity on each channel of the image.
The columns must be separated with a tab, decimals with a ".". 
The table must have column headers with unique column names. 

##### File results.csv 
File containing for each ROI : ID (columns X.1), Area, Mean greyscale, Standard deviation and its X and Y coordinates. 
The table must have column headers with unique column names. 
The columns must be separated with a ",", decimals with a ".".

#### File RoiSet.zip
Zip file containing the ROIs of the image defined with ImageJ.

### Using the application 
#### First step : upload the image you want to analyse 
Use the first item of the menu "Choose your image" and click on the "Browse" button. Select the image you want to analyse in your documents. 

#### Second step : select ROIs to remove
Under the browse box, you can plot variables of the results or the intensity file and select ROIs with extreme values to remove them from the datas to analyse. 
Select the points on the plot and click on the "Remove" button. The ROIs corresponding to these points will be removed from the intensity and result files and from the Roi set. 

#### Third step : plot datas
Use the second item of the menu : "Plot to Image". <br>
Zones of the plot : 
* A plot representing for ROIs their intensities on different channels is displayed. The variables plotted in X and Y can be modified. 
* The plot can be cut in 4 zones : Up Left (UL), Up Right (UR), Down Left (LL) and Down Right (DR) depending on movable horizontal and a vertical lines. At the beginning, all the points have the same color. The colors of the points in each zone can be modified with the button "Reload colors".
* The datas (result file) of the ROIs of each zone can be downloaded in a zip file containing 4 csv files, one for each zone, with the button "Download Groups subtable". 


Selections on the plot :
* Points of the plot can be selected (by clicking or brushing) and datas of the ROIs selected are printed in a table below. 
* These datas can be downloaded in a csv file with the button "Download selected ROIs subtable". 

#### Fourth step : image datas
The image is displayed on the left, channel and slice to display can be modified with the sliders. 
ROIs selected on the plot are displayed on the image and the color of the mask can be modified. 
