# A Comparitive Study of CRNN Architectures for Offline Handwritten Text Recognition

> CSC 8851 Final Project (GSU | Spring 2025)    
> Ana Costa and Srikar Pottabathula

### Setup
In order to train the model in the IPYNB file, the IAM_TrOCR Dataset must be downloaded from the following Kaggle link:    
[https://www.kaggle.com/datasets/changheonkim/iam-trocr](https://www.kaggle.com/datasets/changheonkim/iam-trocr)    
Once the data has been downloaded, place the images and text file in the appropriate folders as illustrated in this file tree:
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
In the IPYNB file, there exists a code block after the `Custom Training loop with CTC loss` code block that allows you to load a pretrained model with weights.    
Instead of training the model again, this code block must be executed in order to replicate the results from the research paper. The code block loads a model with the name `model_03.keras`, which is the model that we proposed in the research paper.    
Unfortunately, GitHub does not allow direct file uploads larger than 25 MB, and so you must download `model_03.keras` from the following Google Drive link and place it in the `saved_base_models` folder as listed in the file tree:    
[https://drive.google.com/file/d/1-5aiZPJKj4bV80HvOe640Q3jXF5uhsd-/view?usp=sharing](https://drive.google.com/file/d/1-5aiZPJKj4bV80HvOe640Q3jXF5uhsd-/view?usp=sharing)    
Currently, there is a blank version of `model_03.keras` called `dummy_model_03.keras`, which is acting as an example/placeholder inside the `saved_base_models` folder since empty directories cannot exist in GitHub repositories.    
**DO NOT** attempt to load `dummy_model_03.keras` because the model will not work. Ensure to download `model_03.keras` from the above Google Drive link and place it in the `saved_base_models` folder in the project directory before attempting to load a model.    
> To avoid `undefined` variable errors, execute all of the code blocks (except the `Custom Training loop with CTC loss` code block) if trying to use the `model_03.keras` model to predict text. Importing the training data is necessary in order to compute the variable `max_W` in the `Computing image height and max width` code block, as it is used while predicting text with the model. If choosing **not** to load the training data to avoid executing the `Computing image height and max width` code block, please define and initialize the variable as `max_W = 4348`, since the maximum width out of all the images is `4348`, and continue execution of the remaining code blocks.

**Ensure all the data files and model files are present in the appropriate folders, and all the directory paths are updated in the IPYNB file to match your project directory before execution.**    

We have also provided two test images (`test_01.jpg` and `test_02.jpg`) that we created personally to mimic the style of the training images. These images are entirely new to the model and have not been used in training, and so, they can be utilized to quickly demonstrate the model's capabilities.

> NOTE: Since this entire project was built in Google Colab, we utilized an easy solution to import files directly from our Google Drive accounts. The `Import Statements` code block in the IPYNB file contains code that prompts the program to connect to a Google Drive account and access the user's Google Drive file system.
> **Avoid executing those statements as it is unnecessary if the IPYNB file is being executed in a local IDE and all the relevant files are locally available in the appropriate folders.**
> Ensure to make the necessary omissions from the `Import Statements` code block and update all the directory paths in the IPYNB file before executing it.

**The model should now be ready to execute block by block as an IPYNB file.**    
If any issues arise while executing the IPYNB file or the model does not function as intended, please contact me (Srikar Pottabathula) at [spottabathula1@student.gsu.edu], and I can assist.
