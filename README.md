# Mucoscope Data Repository

Welcome to Lungs Up's Mucoscope Data Repository! Here you can find our preliminary CAD designs for the stethoscope head, our Python notebook that houses our pneumonia classifier, and the data sets that we trained and tested on.

See our website for more information about our project: 

**Files:**
Pneumonia_Classifier.ipynb: contains the CNN model from Kaggle that we generalized, decomposed, and modularized for ease of use. At the top, the user can modify the parameters that are passed into the "run_analysis" function. This function generates features and labels for a dataset, splits it, and then trains and tests the model. The other user-facing function is "test_only": this function requires a trained model and evaluates a pre-processed test set on this model. Please note that this notebook is still preliminary and so may require minor changes to adapt to a new dataset.

SoundDatasets folder: contains the three data sources of lung recordings we used for our classifier. The table below provides more information on each source:

| Name | Description | Locations of Origin | # of Recordings |
|---|---|---|---|
|Respiratory Sound Database (Rocha_etal)|“920 annotated recordings of varying length - 10s to 90s. These recordings were taken from 126 patients. There are a total of 5.5 hours of recordings containing 6898 respiratory cycles - 1864 contain crackles, 886 contain wheezes and 506 contain both crackles and wheezes.”|Respiratory Research and Rehabilitation Laboratory (Lab3R), School of Health Sciences, University of Aveiro, Aveiro, Portugal;
Papanikolaou General Hospital and the General Hospital of Imathia, Aristotle University of Thessaloniki and the University of Coimbra, Thessaloniki, Greece
|921|
