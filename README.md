# Mucoscope Data Repository

Welcome to Lungs Up's Mucoscope Data Repository! Here you can find our preliminary CAD designs for the stethoscope head, our Python notebook that houses our pneumonia classifier, and the data sets that we trained and tested on.

See our website for more information about our project: 

**CAD folder:** contains our two CAD designs for our stethoscope head that we used for early prototyping. They are built upon the GliaX Stethoscope head design (Github [here](https://github.com/GliaX/Stethoscope))  

**Pneumonia_Classifier.ipynb:** contains the CNN model from Kaggle that we generalized, decomposed, and modularized for ease of use. At the top, the user can modify the parameters that are passed into the "run_analysis" function. This function generates features and labels for a dataset, splits it, and then trains and tests the model. The other user-facing function is "test_only": this function requires a trained model and evaluates a pre-processed test set on this model. Please note that this notebook is still preliminary and so may require minor changes to adapt to a new dataset.

**SoundDatasets folder:** contains the three data sources of pnuemonia lung sound recordings we used for our classifier. We have divided each of the sources into a folder with the recordings ("audio_files") and a file used as the labels ("labels.csv"). The table below provides more information on each source:

| Name | Description | Locations of Origin | # of Recordings |
|:---:|:---:|:---:|:---:|
|Respiratory Sound Database (Rocha_etal)|“920 annotated recordings of varying length - 10s to 90s. These recordings were taken from 126 patients. There are a total of 5.5 hours of recordings containing 6898 respiratory cycles - 1864 contain crackles, 886 contain wheezes and 506 contain both crackles and wheezes.”|Respiratory Research and Rehabilitation Laboratory (Lab3R), School of Health Sciences, University of Aveiro, Aveiro, Portugal; Papanikolaou General Hospital and the General Hospital of Imathia, Aristotle University of Thessaloniki and the University of Coimbra, Thessaloniki, Greece |921|
|Pulmonary (Lungs) Sound (Baghel_etal)|“The pulmonary sound dataset is arranged in two sets: a normal set (11.28%) representing recordings obtained from healthy subjects and an abnormal set (88.72%) containing recordings from pulmonary patients. Each file is 10 s long.”|Fortis Hospital, Vasant Kunj, New Delhi, India|468|
|A dataset of lung sounds recorded from the chest wall using an electronic stethoscope (Fraiwan_etal)|“The overall dataset consisted of a total of 308 lung sound recordings, each of 5 s duration.” “The primary dataset involved a total of 70 patients with different respiratory conditions such as asthma, pneumonia, heart failure, bronchiectasis or bronchitis (BRON disorders), and chronic obstructive pulmonary disease (COPD). Data were also recorded from 35 healthy controls.“|King Abdullah University Hospital, Jordan; University of Science and Technology, Irbid, Jordan|336|

Citations: <br> 
Dutta, Malay Kishore (2022), “Pulmonary (Lungs)  Sound”, Mendeley Data, V1, doi: 10.17632/fr7zvy8j5s.1  <br>
Fraiwan, Mohammad; Fraiwan, Luay; Khassawneh, Basheer; Ibnian, Ali (2021), “A dataset of lung sounds recorded from the chest wall using an electronic stethoscope”, Mendeley Data, V3, doi: 10.17632/jwyy9np4gv.3  <br>
Rocha BM, Filos D, Mendes L, Vogiatzis I, Perantoni E, Kaimakamis E, Natsiavas P, Oliveira A, Jácome C, Marques A, Paiva RP (2018) In Precision Medicine Powered by pHealth and Connected Health (pp. 51-55). Springer, Singapore.
