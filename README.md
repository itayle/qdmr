# The Effect of Data Representation in Question Decomposition
Code for the paper [The Effect of Data Representation in Question Decomposition](The_Effect_of_Data_Representation_in_Question_Decomposition.pdf)


* [About](#About)
    * [Authors](#Authors)
    * [Project](#Project)
    * [Acknowledgements](#Acknowledgements)
* [Project structure](#Project-structure)
    * [Framework](#Framework)
    * [Models](#Models)
    * [Training](#Training)
* [Environment Setup](#Environment-Setup)
# About
This was the final project in the introductory NLP course taught by Prof Jonathan Berant during 2020-2021.

## Authors
The authors of this project are:
- Itay Levy
- Gal Suchetzky

## Project
The [Break It Down](https://github.com/allenai/Break) paper suggested a new decomposition task of a complex question to a series of simple, natural languages steps that can be executed in sequence for answering the original
question. In this project, we investigate the effect of performing the same task with varying
degrees of structured data. We trained several
encoder-decoder models using different types
of gold data representation. Our experiments
show that increasing structurality benefits out-of-distribution generalization significantly.

## Acknowledgements
Prof. Jonathan Berant - Helped with guidance and pointed us to the right people to ask our questions.


# Project structure
## Framework
The base code for this project was adapted from [this](https://github.com/victoresque/pytorch-template) pytorch 
template project.
This framework allows us to define and implement many models, metrics, trainers, testers and data loaders and define 
the combination of the running with a simple, extensible configuration file.

## Models
The models and code used in this project can be found under the 'model/' directory. <br>
Our models were adapted from the course's homework assignments. <br>
We have implemented a very basic model and allowed additional mechanisms to be added using the config files, 
allowing many models that are only slightly different from one another, allowing us to test the contribution of each 
mechanism to the success of the model.

## Training
Training models is as easy as running the train script appropriate configuration file using the following command:<br>
```
python train.py -c config.json
```

# Environment Setup
To setup the environment, do the following steps:
1. Create new conda env with python 3.8
2. Install pytorch with directions from site using pip
3. pip install nlp
4. pip install spacy
5. pip install edit_distance
6. pip install networkx
7. pip install matplotlib
8. pip install torchtext
9. pip install tensorboardx
10. pip install scipy
