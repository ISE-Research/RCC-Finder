# RCC-Finder
## Description
This repository contains all source codes of RCC-Finder, a heuristc code reviewer recommender system. codes folder consists of 7 jupyter notebook. We try to chose each notebook name in a way help to understand its function. 

## structure
Here is  brief explanation of source code files:
  
- WhDo reimplementation: contains reinplementation of WhoDo, the recommender system with which we compare our proposed approach.
  
- preparetion: contains code of some primary data modifications, such as selecting pull requests which has been reviewed and finding all candidate reviewers.
  
- relative scores calculation: Basic commit and review scores are obtained in WhoDo reimplementation. In this file we caculate relative commit and review scores based on 
  those   basic ones. 
  
- former packs change score: WhoDo consider commit experience on files and last level directories. In this file we try to test commit score for direcories in the level 
  preceding the last level.
  
- review and commit scores calculation with different time coefficients: RCC-finder consider recency of commit and review experiences. This file contains source code for   
  calculating scores using different time coefficients. 
  
- calculate collaboration score: contains source code for calculating collaboration score.
  
- calculate activity score using 5 different methods: contains of five different methods we tried to calculate activity score through
  
## Dataset

Our dataset is accessibe through Zenodo link bellow:

[Dataset](https://zenodo.org/records/10669853?token=eyJhbGciOiJIUzUxMiJ9.eyJpZCI6ImZjM2I3ZGQyLTkwMWEtNGE5Ny05N2M4LThjNmFiMzEzZWMwZiIsImRhdGEiOnt9LCJyYW5kb20iOiJmYzMxMDQzN2VlMDBkMjkwYWQxNDYxOTJlMDkxZTI2NiJ9.1iBnDz1Ac_94s8gamLULyl4nFji03fxGNQUFKJqojmrXaNHCdFHUy37BuP4d4bkiQGkhvUxcUDQK7Dn-RxkR3g)

The repository consists of two folders: 
- dataset which contains the primary dataset of article [] we used companion with additional data we fetched using GitHub rest API. 
  
- features: contains sheets of data represents different combinations of original dataset we created to facilitate scores calculations.
  
In code files we read dataset and features files content refering by address. We assume which dataset and features folders are in the same folder as jupyter notebooks. Also, our codes make some new files in a new directory beside notebooks named results.
