# Solar Flare Prediction
Using machine learning and data science, this project is using solar data obtained publicly from the NOAA, GOES-15 (satellite) multivariate time-series data, to predict the class of a solar flare as they happen on Sol. X-Ray Sensors (XRS) which are present on the GOES-15,  provides solar X-ray irradiances for the wavelength bands of 0.5 to 4 ˚A (short channel) and 1 to 8 ˚A (long channel).


The X-ray irradiance *W* in each channel is calculated as:
***Irradiance [W m−2] = (Counts − B) × G/C (1)***
where *B* is the background, *G* is the gain, and *C* is the units conversion factor. 


Data for this project can be found here: https://drive.google.com/drive/folders/1ZIGNgBmsaFaN4IuyXvtmb8h_ToCHPIZW?usp=sharing

The data can also be obtained from https://www.ncei.noaa.gov/data/goes-space-environment-monitor/access/science/xrs/goes15/ . The author has used IRRAD and FLSUM data, specifically the compiled data found when *gxrs-l2-irrad_science/* or *xrsf-l2-flsum_science/* is opened on the aforementioned website.

A readme file for the further details about how the data is obtained and further explanation about GOES-15 is present here: https://www.ncei.noaa.gov/data/goes-space-environment-monitor/access/science/xrs/GOES_1-15_XRS_Science-Quality_Data_Readme.pdf

The data exists in a .rar file. To use the data, please extract the folders within and place it in the same directory as the Python notebook. If needed, please do change the location specified in the code to point it to the correct location of the data.


To use this project, make sure to set up and run multiyear_models.ipynb, as this notebook contains the code to preprocess and transform the data into the multi-year dataset that will be used to train and evaluate the models. In the notebook, there is a parameter called YEARS in which the user must specifiy which years they would like to use. Reccomended is 2015, 2016, 2017.
