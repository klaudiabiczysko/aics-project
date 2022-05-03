# aics-project

Project for Artificial Intelligence: Cognitive Systems class.
authors:  Klaudia Biczysko & Justyna Sikora
## Table of contents
* [Short description](##Shortdescription)
* [Dataset](##Dataset)
* [Outline](##Outline)
* [Results](##Results)
* [Conclusions](##Conclusions)
* [Citation](##Citation)

## Short description
In this folder, we present jupyter notebooks for:
- Classification based on title using BERT (Text model.ipynb)
- Classification based on cover image using ResNet (Image model.ipynb)
- Classification based on BERT+ResNet (Text + image.ipynb)

To run BERT+ResNet, models BERT and ResNet need to be saved. The obtained models were not included in the repository due to size constraints. 

## Dataset
For this project, we used the [Uchida Book Dataset](https://github.com/uchidalab/book-dataset/tree/master/Task1) containing data from approximately 57,000 Amazon books. This dataset contains images of book covers, titles, authors, and subcategories for each book. Each book is divided into 30 categories.

To access the dataset, clone the repository:

```sh
#downloading dataset
!git clone https://github.com/uchidalab/book-dataset.git
%cd ./book-dataset/Task1
!ls 
```
## Results
| Classifier | Accuracy |
| ------ | ------ |
| BERT | 58.5% |
| ResNet50 | 30% |
| BERT+ResNet50 | 23.9% |

For the BERT+ResNet50, we also calculated top-3 accuracy (42.2%) and top-5 (53.5%).

## Conclusions
As a result of our findings, we can conclude that our way of concatenating BERT with ResNet produced a very deep and complex model. We were not able to achieve satisfactory results and increase the accuracy scored by BERT or ResNet.

## Citation
[1] B. K. Iwana, S. T. Raza Rizvi, S. Ahmed, A. Dengel, and S. Uchida, "Judging a Book by its Cover," arXiv preprint arXiv:1610.09204 (2016).

[2] The code for ResNet was adapted from [Pytorch manual](https://pytorch.org/tutorials/beginner/transfer_learning_tutorial.html).

[3] The code for BERT was adapted from [Medium](https://towardsdatascience.com/text-classification-with-bert-in-pytorch-887965e5820f).
