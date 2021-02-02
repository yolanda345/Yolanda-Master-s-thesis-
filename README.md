# Master-s-thesis-
Datasets and code for thesis project work. Each file contatains datsets used and preprocessing code files.

A short description of each file is provided below. However, each stage of the preprocessing techniques is described step by step in the thesis document.

### Weather data preprocessing 
The ***original datasets*** file includes the raw data files for both temperature and rainfall datasets of the Grootfontein compartment. ***Grootfontein_weather.xlsx*** contains the combined raw temeprature and rainfall datasets. ***Combining weather.ipynd*** file contains code were we average the rainfall and temperature datasets to obtain a master weather dataset to later be used for modelling ***(precipitation.xlsx and temperature.xlsx)***. Some anaysis of the individual datasets is also done in the file (code decsriptions are also provided in the ***ipynb*** bile).  

### Usage data preprocessing 
***Grootfontein 2016 (original full dataset).csv*** contains the raw dataset obtained from WARMS. However, some of the datapoints fall outside the defined study boundary so we had to filter the boreholes by latitude and longtitude to select only those inside the study area (this was done in qgis) and the resultant file from this was the ***Grootfontein 2016 (original dataset but within boundary).csv***. Preprocessing was done in order of **.ipynb files** and each stage gives a resulting **.xlsx file**. The final file used in modelling is ***2016 monthly usage.xlsx***


### Discharge data preprocessing
Files ***D4H013.xlsx*** and ***D4H014.xlsx*** are the raw data files of the 2 discharge stations found in the aquifer. ***grootfontein gauge data.ipynb*** contained the preprocessing steps done to the discharge data explained in thesis document and the resulting excel file used for modelling is ***Discharge.xlsx***

### Groundwaterlevel (gwl) data preprocessing
This was a little more complex as datasets obtained were in bad shape. Each step (1,2,3 ..., 6) is defined in detail in the thesis document. To preprocess the data we will need to go step by step of the defined **.ipynb files**. After step 6 (clustering data points) we get the ***master spreadsheets for compartment per cluster*** file which contains the individula clusters that were used for modelling.

### Final models

In this file we have the preprocessed final datasets all in one place (***master spreadsheets***). These are the files which are called in the **.ipynb files** during model development. Cross correlation was also done between each variable and all grounwater level boreholes. The resultant images of this are found in the ***cross correlation*** file. Lastly, the **.ipynb files** found in ***final models*** folder are the python files were we model each indiviudual borehole. Detained descriptions are also provided in code. 

### Raw datasets
During data aquistion datsets were obtained for 6 regions in South Africa (Grootfontein, Steenkoppies, Turfontein, Zuukerbum, Schroonspruit and Elandfontein ). All the obtained raw datasets are found in this file. To see the location of each dataset you will need to plug in the latitude and longitude coordinates in qgis. I have included the latitude and longtitue for all varibales file to make this process easier. I have also included the shape files needed for qgis (***Files for qis*** >> ***North west shape files***). 

**For detailed descriptions of preprocessing stages refer to chapter 3.4 in thesis and for detailed description of model development refer to chapter 4.2 of thesis**
