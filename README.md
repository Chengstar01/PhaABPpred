# PhaABPpred
Predicting antibacterial peptides in bacteriophage using attention-based Siamese network


## Introduction
In the study, a phage-specific prediction method was proposed, PhaABPpred, to predict ABPs from sequences, using a Siamese neural network architecture that incorporates an attention mechanism. This work has the following advantages over existing methods:  
(1) A deep learning model called PhaABPpred for predicting PhaABPs from protein sequences, which uses an attention-based Siamese neural network to optimize feature learning.  
(2) The model outperformed other classifiers on the test set in terms of accuracy, F1 score, etc.   
(3) We have used this model to discover new PhaABPs by applying it to the phage genome.
(4) A freely accessible web server was built using the model, where we can input protein sequences and get the predictions given by our model.


## Related Files

#### PhaABPpred

| FILE NAME         | DESCRIPTION                                                                               |
|:------------------|:------------------------------------------------------------------------------------------|
| prediction.py     | the main file of PhaABPpred predictor (include data reading, encoding, and model loading) |
| dataset           | used data                                                                                 |
| feature_generation| generating features                                                                       |
| iFeature          | call the local dependency package to compute the feature matrix                           |
| model             | model construction and loss functions used to train models                                |
| model_save        | the trained model saved                                                                   |
| results           | saving predicted results                                                                  |
| temp_blosum_file  | temp blosum62 feture matrix                                                               |



## Installation
- Requirement
  
  OS：
  
  - `Windows` ：Windows10 or later
  
  - `Linux`：Ubuntu 18.04.6 LTS or later
  
  Python：
  
  - `Python` >= 3.8
  
- Download `PhaABPpred-main.zip`to your computer

- open the dir and install `requirements.txt` with `pip`

  ```
  cd PhaABPpred
  pip install -r requirements.txt
  ```
  
## Predicting by using PhaABPpred model
```shell
cd "./PhaABPpred/"
updating input file name in load_data("input_file.fasta")
python prediction.py
```


## Getting results
```
Open "results.csv" in the results directory to see and download the predicted results
```


## Contact
Please feel free to contact us if you need any help.

