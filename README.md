# A Comparitive study of CRNN Architectures for Offline Handwritten Text Recognition

> CSC 8851 Final Project (GSU | Spring 2025)    
> Ana Costa and Srikar Pottabathula

### Setup
In order to execute the IPYNB file, the IAM_TrOCR Dataset must be downloaded from the following link:
[https://www.kaggle.com/datasets/changheonkim/iam-trocr](https://www.kaggle.com/datasets/changheonkim/iam-trocr)    
Once the data has been downloaded, place the data in the appropriate locations like so:
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
Instead of training the model again, this code block must be executed in order to replicate the results from the research paper. The code block loads a model with the file name `model_03.keras`, which is the model that is we proposed in the research paper.

Ensure all the data files and model files are present in the appropriate folders and all the directory paths are updated in the IPYNB file before execution.
The model is now ready to be executed block by block as an IPYNB file.
