# SeaIceConcentration_EMPE

# Sea Ice concentration metadata file 
#Mean and standard deviation of sea ice concentration values within 200km of the seven emperor penguin colonies in the Ross Sea, 
#and the overall Ross Sea region (165E-150W, 65S-79S)
#Eight Regions of Interest (ROIs) created in ArcGIS Pro. 
#Using latitude and longitude points for each penguin colony and creating a 200km buffer around each point and excluding the area covered by continent. 
#Ross Sea ROI was created using ‘Go to XY’ function, placing markers at 165E-150W, 65S-79S, drawing a polygon between the points, 
#then excluding areas covered by continent. 

#Sea ice concentration geotiff data were gathered through NSIDC (https://masie_web.apps.nsidc.org/pub/DATASETS/NOAA/G02135/south/monthly/geotiff/) 
#Images are 25 km data cell color-coded in shades of blue to white, where dark blue is zero percent ice (open ocean) and white is 100 percent ice. 
#We wanted to extract the mean sea ice coverage within each of our ROIs, and calculate the ‘seasonal’ (or three-monthly) averages and standard deviations. 
#This was done in R. 
#Our seasons are Jan-Feb-Mar (JFM), Apr-May-Jun (AMJ), Jul-Aug-Sep (JAS), & Oct-Nov-Dec (OND). 
#These were chosen as each three month period relates to a different aspect of the emperor penguin lifecycle.

#We extracted the monthly sea ice concentration data using the ROIs in R, before creating a variable with dates month, year and season. 
#We were then able to take the mean and sd of the seasons for each year from 2000-2021


