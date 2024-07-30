# Precise Flight

Preciseflight is a tool used for post-flight analysis that enables operators to run PPK on imagery collected with Powered-by-Auterion Vehicles. Users can select the required data folders from the main page.





<figure><img src="../../.gitbook/assets/main.png" alt=""><figcaption></figcaption></figure>



### Mission Data

This folder has to contain the images taken during the survey. In particular, the folder has to contain the following description files:

* sequence.json file containing the sequence of the images.
* \*.obs file&#x20;
* imagelog.json file containing the log of the images.

When you select a folder that does not contain one of those files the software will show a popup with the error message like the following:





<figure><img src="../../.gitbook/assets/spaces_7S1QElc9VpiBzRbPAWCp_uploads_57uUU9YWoqjWb2pcnmaj_error_missing_pictures.webp" alt=""><figcaption></figcaption></figure>

### Base Station Data



This folder has to contain the RINEX files matching the following file format name: .digit digit letter.



### Saves images in





<figure><img src="../../.gitbook/assets/folder_not_empty.png" alt=""><figcaption></figcaption></figure>

### Select Base Station Position

Clicking on the ">" in the bottom right corner you'll gain access to the select base station position input window

From this section you can select one of the following methods to insert the base station position:



* **Manual**
* LLH
* Rinex

For best Accuracy results, inputting manually the base station position is recommended.

#### Manual

As the name stands, you can insert the latitude, longitude, and altitude of the base station position. Then just click on Set base position to accept the position.





<figure><img src="../../.gitbook/assets/spaces_7S1QElc9VpiBzRbPAWCp_uploads_VyHoMDEdrTP6ZG9XogLt_Screenshot from 2023-11-10 15-51-18.webp" alt=""><figcaption></figcaption></figure>

LLH

In this mode, you can select a LLH file logged by the base station (E.g Emlid RS2) in order to set the base station position. Precise Flight will average the position and show the result on the map.



<figure><img src="../../.gitbook/assets/spaces_7S1QElc9VpiBzRbPAWCp_uploads_SgcktOqOVLApbLgy5k6W_Screenshot from 2023-11-10 15-50-34.webp" alt=""><figcaption></figcaption></figure>

Selecting a valid.LLH file you'll get a confirmation popup like the following one:





<figure><img src="../../.gitbook/assets/spaces_7S1QElc9VpiBzRbPAWCp_uploads_caY2rlzaLqd9x2ScAyAw_Screenshot from 2023-11-10 15-49-41.webp" alt=""><figcaption></figcaption></figure>

By clicking on confirm the current base station position will be set to the imported one.



#### RINEX

Selecting RINEX the base station position will be read from the observation file header.

<figure><img src="../../.gitbook/assets/spaces_7S1QElc9VpiBzRbPAWCp_uploads_zCiNDoKP4V4Kd5CxMfm2_Screenshot from 2023-11-10 15-51-11.webp" alt=""><figcaption></figcaption></figure>

Based on our testing, this solution does not generate high-accuracy results.

### Process

Once you have selected all the required files, the button Process will be active and you can proceed with the PPK.



<figure><img src="../../.gitbook/assets/spaces_7S1QElc9VpiBzRbPAWCp_uploads_ZdNKljL2Ty7pw8b3XNOt_Screenshot from 2023-11-10 15-47-24.webp" alt=""><figcaption></figcaption></figure>

Then, the process is completed, a trajectory will be loaded on the map as follows:



<figure><img src="../../.gitbook/assets/spaces_7S1QElc9VpiBzRbPAWCp_uploads_2ewTB1GfE74m99tQUGcG_Screenshot from 2023-11-10 15-48-29.webp" alt=""><figcaption></figcaption></figure>



Events that can't be geotagged will be flagged with a red dot.
