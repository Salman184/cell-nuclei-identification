# Cell Nuclei Identification
A deep learning project to identify different types of cell nuclei in a colon cancer sample.

 <img src="https://user-images.githubusercontent.com/66486975/147992105-ee3f4abd-8b87-41b4-8259-bc5be01f3066.png" width="250" height="250">

This is a simple deep learning project to train a deep neural network that can take a 64x64 image with cell nuclei at the centre and classify it into one of the following types which are shown in the figure above:
1.	Normal epithelial cells (shown orange).
2.	Cancer epithelial cells (shown in red).
3.	Immune Leukocyte cells (shown in green).
4.	Connective fibroblast cells (shown in blue).

## Requirements Installation
Create a conda virtual environment to install and run the code using the command:
```shell
conda create -n cellNucleiIdentify_env
```
Activate the environment using the command:
```shell
conda activate cellNucleiIdentify_env
```
Install the required packages in the requirements.txt file using the command:
```shell
pip install -r requirements.txt
```

## Run Code
- The training set of nuclei images `train.zip` and a csv training file `train.csv` containing their identities are present in [data] folder. This folder also contains test archive `test.zip` which has similar 64x64 images of unlabelled cell nuclei.  
- Unzip those training and test images to a repository.  
- Run the provided `cellNucleiIdentify.ipynb` notebook file in the same repository.  

## Model Evaluation and Validation
The model is evaluated by predicting the cell type of the images in the `test.zip` file.

The training and testing accuracy and the corresponding training and testing loss at each epoch is plotted as follows:

![image](https://user-images.githubusercontent.com/66486975/147995693-73204ba1-b95e-4ccf-b295-6a77d387a61e.png)&nbsp;&nbsp;&nbsp;&nbsp;
&nbsp;&nbsp;&nbsp;&nbsp;![image](https://user-images.githubusercontent.com/66486975/147995706-4c858380-f27f-4eb8-b00b-a1ee6c9475c3.png)

| Image Set | Accuracy |
| --------- |:--------:|
| Train Set | 78.586%  |
| Test Set  | 75.208%  |
