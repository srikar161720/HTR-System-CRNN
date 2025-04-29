# A Comparitive study of CRNN Architectures for Offline Handwritten Text Recognition

> CSC 8851 Final Project (GSU | Spring 2025)    
> Ana Costa and Srikar Pottabathula

### Setup
In order to execute the IPYNB file, the IAM_TrOCR Dataset must be downloaded from the following link:
[https://www.kaggle.com/datasets/changheonkim/iam-trocr](https://www.kaggle.com/datasets/changheonkim/iam-trocr)    
Once the data has been downloaded, place the data in the appropriate folders like so:
```
|--- HTR_final_project.ipynb
|--- gt_test.txt
|--- saved_base_models
     |--- model_03.keras
|--- images
     |--- < 2,915 image files >
|--- personal_test_images
     |--- < personal test image files >
```
In the IPYNB file, there exists a code block after the training loop code block that allows you to load a pretrained model with weights.
Instead of training the model again, this code block must be executed in order to replicate the results from the research paper. The code block loads a model with the file name `model_03.keras`, which is the model that we proposed in the research paper.

> NOTE: Since this entire project was built in Google Colab, Google Drive provides an easy solution to import files from a user's account. The `Import Statements` code block in the IPYNB file contains code that prompts the program to connect to a Google Drive account and access the user's Google Drive file system. Those statements are unnecessary if your data files and model files are locally available in the appropriate folders. Ensure to make the necessary omissions from the `Import Statements` code block and update all the directory paths in the IPYNB file before executing it.

Ensure all the data files and model files are present in the appropriate folders, and all the directory paths are updated in the IPYNB file to match your project directory before execution.

The model is now ready to be executed block by block as an IPYNB file.
