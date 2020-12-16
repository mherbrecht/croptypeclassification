# croptypeclassification

The code published here was written as part of my master's thesis, which deals with crop classification from multitemporal radar imagery from the Sentinel-1 satellite without training data in the cloud (Google Earth Engine).

Satellite-based remote sensing is an effective and inexpensive tool for monitoring and mapping large areas. Due to the high annual dynamics of agricultural land, very high temporal resolution of data is required. This is provided by synthetic aperture radar (SAR) sensors such as Sentinel-1, which operate independently of cloud cover. Most approaches use mapped training datasets for supervised classifications of crop species. However, the required mapping campaigns are costly and time consuming. Therefore, a work process without training data would be a significant improvement.

In my master thesis, a multitemporal decision tree based unsupervised classification approach is developed and validated. It requires no training data and incorporates knowledge about the temporal variation of crop backscatter due to phenological changes. The study area is that of the Transregio Collaborative Research Center 32 (www.tr32.de), which covers the area of the Rur watershed of about 1500 km² in western Germany, Belgium and the Netherlands. Within the framework of the research project, in the last few years, cultivar classifications have been continuously carried out with supervised classifications of mainly optical remote sensing data. Thus, the study area is an optimal location to evaluate the approach developed in the present work. The typical crops in the study area are winter wheat, winter rye, winter and summer barley, canola, corn, sugar beets and potatoes.

Prior to implementation of the algorithm, the annual backscatter variations of the typical crops in the study region were evaluated by constructing time series plots. These were then used to derive classification decision rules for classifying the Sentinel-1 backscatter time series into the above crops. 

An accuracy study of the classification results over three years using standard error matrices and comparison classifications looks very promising. For example, canola can be excellently separated from all other crops and winter and summer crops can be efficiently distinguished. In general, the overall accuracies are around 87 to 91 %, with some readjustments still required within the individual classes.

If you don't want to play with my code, but just want to run a classification, use the buttons in the console. There you can select the year, the area and if you want to use a mask. But take everything outside the tested approach and area with caution.



