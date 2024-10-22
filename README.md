This code was produced for the IBMz 2024 Datathon with an aim to make Dyslexia diagnosis available, on hand, to all. By analysing the handwriting of a person, it is possible to determine the likelyhood of an individual having dyslexia.
The user can submit an image of their handwriting to the model, and then view plots of their writing against the test dataset where positive and negative diagnosises can be seen clearly. 

This was run on IBMs LinuxOne cloud platform, using a jupyterlab interface held in a docker, which also makes use of IBMs built-in machine learning accelerator.

In this case, the gpt4 API is called with images for computer vision to collect the datapoints: Number of incorrect spellings, number of case errors, joining, legibility and line alignment in handwriting. 
These points are put into a logistic regression algorithm trained on labelled handwriting data from traditionally diagnosed individuals. 

Notes for running the code: 

**Please use this API Key, the one in use on the notebook is deprecated** sk-O3Gi2vYo9zU68apskGpVpy93E6EjkK2K7mL-uRpRo1T3BlbkFJbYGPQKMnDrVhVTGr4zzgztEwkUC_lC-TSSmFTtXwUA

Additionally, please follow these steps to analyse your handwriting: 
  1) Drag your handwriting sample photo (.jpg, .jpeg, .png) into the same directory as the main DYSLEIXAI.py file.
  2) when the program runs, you will be asked for the path of your handwriting sample please provide the appropriate file name e.g. handwritingsample.png.
 
