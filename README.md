# SES_LSTM
Modified LSTM for Smart Eyedrop System Project

## Platform
- Code had been compiled using Spyder via Anaconda platform. 
- For terminal, use the following command to install necessary packages:
	- pip install keras 
	- pip install tensorflow
	- pip install sklearn
	- pip install matplotlib
	- pip install pandas
	- pip install flask
           
## Models
- Neutral Model: Trained on 100 entries, Tested on 100 entries
- Base Model: Trained on 50 entries, Tested on 50 entries
- Heavy Model: Trained on 250 entries, Tested on 300 entries
> 'combineROC' and 'LSTMReport' are visualization functions. Comment them out if you want the model by itself.

## Connection via Flask
- By default, code is independent of rest of SES. To reconnect, uncomment 'Flask Connection' code block.

## Data
- Data is separated by kurtosis, min, max, mean, and median values
	- Each value is seperated by x, y, and z axis
- Each entry is assigned one of 6 different labels
	- Label 0 is given to random movement
	- Label 1 is given when the eyedropper is applied once
	- Label 2 is given when the eyedropper is applied twice
	- Label 3 is given when the eyedropper is dropped
	- Label 4 is given when the eyedropper is lifted but not used
	- Label 5 is given when the user walks with the eyedropper

## Original SES
- Instructions for running the original Smart Eyedrop application can be found here: https://github.com/EilonwyLlyr/SED_backend
