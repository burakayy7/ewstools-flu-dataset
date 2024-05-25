# ewstools-flu-dataset

This is an implementation of the [ewstools](https://github.com/ThomasMBury/ewstools) library for predicting critical transistions on a US Flu data.

The CSD and DL based code was directly used from the [documentation of the library](https://github.com/ThomasMBury/ewstools/blob/main/tutorials/tutorial_deep_learning.ipynb)

## Data Used
The flu data is from [this](https://raw.githubusercontent.com/cdcepi/FluSight-forecast-hub/main/target-data/target-hospital-admissions.csv) dataset.

## Colab Notebooks
Everything is implemented in the [Colab Notebook](https://github.com/burakayy7/ewstools-flu-dataset/blob/481fc23054379e5c6c36e0ad6eeec4ff68b71aa1/EWS_Flu.ipynb). Also, in a seperate notebook, I have computed various CSD based values and have added them to a Pandas DataFrame [Colab Notebook for CSV data output](https://github.com/burakayy7/ewstools-flu-dataset/blob/d4a61e29ed0f8bc197e6988a2d728f2d66925f6a/EWS_Flu_CSV.ipynb), which was then converted to a [CSV file](https://github.com/burakayy7/ewstools-flu-dataset/blob/077f22dbd37c685f4e5ae1073e683983757e32f3/data.csv) (the first few CT values will be empty, as there needs to be some past p-lagged values inorder to compute values like Autocorrelation).

*Diclamer: It seems that there is an error when we try to plot the average DL predictions accross different classifiers. I got this code from the official turorials and documentation of the ewstools library, however, I think there is a bug in the library code. I couldn't figure out why this error was coming up.

Please reach out if you have any suggestions!
