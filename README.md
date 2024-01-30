## Image Forgery


This data science project focuses on the development and implementation of a deep learning-based solution for identifying tampered regions within digital images, an essential task in fields like digital forensics and multimedia security. At the heart of the project is the U-Net architecture, a convolutional neural network originally designed for biomedical image segmentation. The choice of U-Net is motivated by its exceptional ability to capture fine details and its efficiency in learning from a limited amount of labeled data.

The project involves several key phases: data preprocessing, model training, ablation study and evaluation. The data used is [CoMoFoD](https://www.vcl.fer.hr/comofod/), a small dataset of original and tampered images along with their masks and some augmented images, ensuring a wide range of manipulation techniques are represented. In this project, another set of techniques was used. Preprocessing steps include resizing images, normalizing pixel values, and augmenting the dataset to improve model generalizability.

The core of the project is the adaptation and training of the U-Net model to recognize and delineate tampered regions in images. The U-Net's architecture, with its symmetrical contracting and expansive paths, enables precise localization and is fine-tuned to optimize performance for the specific task of tamper detection.

Evaluation of the model's performance involves quantitative metrics such as accuracy and mean IoU metrics, as well as qualitative analysis through visual inspection of the segmented regions in test images. The project aims to achieve a high level of accuracy in detecting a wide range of tampering techniques like cloning.


## Project Organization

    ├── LICENSE
    ├── README.md          <- The top-level README for developers using this project.
    │
    │
    ├── models             <- Trained and serialized models, model predictions, or model summaries
    │
    ├── notebooks          <- Jupyter notebooks. 
    │
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    │
    ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── figures        <- Generated graphics and figures to be used in reporting
    │
    └── requirements.txt   <- The requirements file for reproducing the analysis environment



--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>
