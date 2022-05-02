# aics-project

Project for Artificial Intelligence: Cognitive Systems class.
authors:  Klaudia Biczysko & Justyna Sikora
## Table of contents
* [Short description](##Shortdescription)
* [Dataset](##Dataset)
* [Outline](##Outline)
* [Citation](##Citation)

## Short description
For this project, we decided to compare whether it is easier to predict a category of book given a title, or given a cover. Moreover, we tried to concatenate our two trained models (BERT+ResNet) to see if we are able to boost up the accuracy of the model.

This project is divided into three parts:
- Classification based on title using BERT
- Classification based on cover image using ResNet
- Classification based on ResNet+BERT

## Dataset
For this project, we used the [Uchida Book Dataset](https://github.com/uchidalab/book-dataset/tree/master/Task1) containing data from approximately 57,000 Amazon books. This dataset contains images of book covers, titles, authors, and subcategories for each book. Each book is divided into 30 categories.
| Label | Category |
| ------ | ------ |
| 0 | 	Arts & Photography |
| 1 | Biographies & Memoirs |
| 2 | 	Business & Money |
| 3 | Calendars |
| 4 | 		Children's Books |
| 5 | Comics & Graphic Novels|
| 6 | 	Computers & Technology |
| 7 | Cookbooks, Food & Wine |
| 8 | Crafts, Hobbies & Home |
| 9 | Christian Books & Bibles |
| 10 |Engineering & Transportation |
| 11|	Health, Fitness & Dieting |
| 12|	History	 |
| 13|	Humor & Entertainment|
| 14|	Law |
| 15|	Literature & Fiction |
| 16	|Medical Books |
| 17	|Mystery, Thriller & Suspense |
| 18	|Parenting & Relationships |
| 19	|Politics & Social Sciences |
| 20	|Reference |
| 21	|Religion & Spirituality |
| 22 |	Romance |
| 23 |	Science & Math|
|24 |	Science Fiction & Fantasy|
|25 |	Self-Help |
26	| Sports & Outdoors
|  27 |	Teen & Young Adult |
| 28|	Test Preparation |
| 29|	Travel |


To get dataset, clone the repository:

```sh
#downloading dataset
!git clone https://github.com/uchidalab/book-dataset.git
%cd ./book-dataset/Task1
!ls 
```

## Outline
```
├── aics-project
│   ├── code
│   │   ├──   Image model.ipynb
│   │   ├──   Text + image.ipynb
│   │   ├──   Text model.ipynb
│   │   ├──   readMe.md
│   ├──  notes
│   │   ├──   readMe.md
│   │   ├──   slurm-5810705_epoch5.out
│   │   ├──   slurm-5810732_epoch10
│   ├──  paper
│   │   ├──   KBiczysko_JSikora_aics_final.pdf
│   ├──  plots
│   │   ├──   output_matrix_bert.png
│   │   ├──   output_matrix_multimodal.png
│   │   ├──   output_matrix_resnet.png
├── readme.md
```
## Citation
[1] B. K. Iwana, S. T. Raza Rizvi, S. Ahmed, A. Dengel, and S. Uchida, "Judging a Book by its Cover," arXiv preprint arXiv:1610.09204 (2016).
