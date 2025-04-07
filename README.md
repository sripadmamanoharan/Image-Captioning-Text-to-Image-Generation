# Image Captioning Project

## Code Execution Steps
1. We have used the Flickr30k dataset for training, so it is important that this dataset is present in executing the project code. The dataset is available on Kaggle in the [Link](https://www.kaggle.com/datasets/hsankesara/flickr-image-dataset). Upon downloading the dataset place the dataset within the same direcory as the code files and make sure the folder will be named as `data`. Upon extracting the code files and data the folder structure should look like -
```
.
├── data
│   ├── flickr30k_images
│   └── results.csv
├── exp-baseline-12-layesr.ipynb
├── exp-basline.ipynb
├── exp-effb0.ipynb
├── exp-effb1.ipynb
├── exp-effb2.ipynb
├── exp-effb3.ipynb
├── exp-inc-v3.ipynb
├── exp-inc-v4.ipynb
├── exp-long-seq-baseline.ipynb
├── exp-long-seq-resnet34.ipynb
├── exp-small-vocab-12-layers.ipynb
├── exp-small-vocab-baseline.ipynb
├── exp-small-vocab-freq-filter.ipynb
├── exp-swin.ipynb
├── exp-vit.ipynb
├── final-model.ipynb
├── README.md
└── requirements.txt
```

2. To run the program first make sure that the required packages are installed. The required packages are present in the file `requirements.txt`. To install the packages run the command - `pip3 install -r requirements.txt`.

3. Upon installing the packages to run these files as they are present in Jupyter Notebook format you either use Jupyter Lab or Jupyter Notebook environment to execute the code. In the `requirements.txt` file we have mentioned the `jupyterlab` package, so I would recommend to run these notebooks in a Jupyter Lab environment. So to run the Jupyter Lab run command - `jupyter lab`

4. You can run the cells and after the model training is complete you should see the resulting weights file (`.pth`) and execution runs generated captions