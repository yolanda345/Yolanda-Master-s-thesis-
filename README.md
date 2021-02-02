# Master-s-thesis-
Datasets and code for thesis project work

Each file contatains datsets used and preprocessing code files.

Esch stage of the preprocessing techniques is decriped step by step in the thsis document. Here a short descriotion is given.

### Weather data preprocessing 
The original datasets include the raw data files for both temperature and rainfall.*Grootfontein_weather.xlsx* conatins the combined raw temeprature and rainfall datasets. *Combining weather.ipynd* file contains code were we average the rainfall and temperature datasets to obtain a master weather datset to later be used for modelling (precipitation.xlsx and temeprature.xlsx). Some anaysis of the individual datasets is also done in the file.  

### Usage data preprocessing 
*Grootfontein 2016 (original full dataset).csv* contains the raw dataset obtained from WARMS. However some of the dataspounts do not fall within the study area so we had to fileter the latitude and latitude to only those inside the study area (done in qgis) and the result file is *Grootfontein 2016 (original dataset but within boundary).csv*. then preprocessing is done in order of ipynb files and each stage gives a resulting xlsx file. The final file used in modelling is *2016 monthly usage.xlsx*


### Discharge data preprocessing
Files *D4H013.xlsx* and *D4H014.xlsx* are the raw data files of the two discharge stations found in the aquifer. *grootfontein gauge data.ipynb* contained the preprocessing steps done to the discharge data explained in thesis document and the resulting excel file used for modelling is *Discharge.xlsx* 

### Groundwaterlevel (gwl) data preprocessing
This was a little more complex as datasets obtained were in bad shape. Each step (1,2,3 ...6) is defined in detail in the thesis document. To preocess the data we will need to go step by step of the defined *.ipynb* files. After step 6 (clustering data points) we get the *master spreadsheets for compartment per cluster* file which is used for modelling

### Final models

In this file we have the preprocessed final datasets all in one place (*master spreadsheets*). These are the files which are called in the *.ipynb* files during model development. Cross correlation was also done between each variable and all grounwater level boreholes. the resultant images of this are found in the *cross correlation* file. The *.ipynb* files found in final models folder are the python files were we model each indiviudual borehole. Detained descriptions are also provided in code. 

### Raw datasets
During data aquistion datsets were obtained for 6 regions in South Africa (Grootfontein, Steenkoppies, Turfontein, Zuukerbum, ). All the obtained raw datasets are found in this file. To see the location of each dataset you will need to plug in the latitude and longitude coordinates in qgis. I have included the latitude and longtitue for all varibales file to make this process easier. I have also included the shaoe files need in qgis *Files for qis* >> *North west shape files*. 
