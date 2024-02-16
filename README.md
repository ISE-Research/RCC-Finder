# RCC-Finder
## Description
This repository contains all source codes of RCC-Finder, a heuristic code reviewer recommender system. The codes folder consists of 7 jupyter notebooks. We tried to choose each notebook name in a way that helped to understand its function. 

## structure
Here is a brief explanation of source code files:
  
- WhDo reimplementation: Contains reimplementation of WhoDo, the recommender system with which we compared our proposed approach.
  
- Preparation: Contains code of some primary data manipulations, such as selecting pull requests that have been reviewed and finding all candidate reviewers.
  
- Relative scores calculation: Basic commit and review scores were obtained in the WhoDo reimplementation. In this file, we calculated relative commit and review scores based on those basic ones. 
  
- Former packs change score: WhoDo considers commit experience on files and last-level directories. In this file, we tried to test the commit score for directories in the level preceding the last level.
  
- Review and commit scores calculation with different time coefficients: RCC-finder considers recency of commit and review experiences. This file contains the source code for   
  calculating scores using different time coefficients. 
  
- Calculate collaboration score: Contains source code for calculating collaboration score.

- Calculate activity score using 5 different methods: contains of five different methods we tried to calculate activity score through.
  
## Dataset

Our dataset is accessible [here](https://zenodo.org/records/10669853?token=eyJhbGciOiJIUzUxMiJ9.eyJpZCI6ImZjM2I3ZGQyLTkwMWEtNGE5Ny05N2M4LThjNmFiMzEzZWMwZiIsImRhdGEiOnt9LCJyYW5kb20iOiJmYzMxMDQzN2VlMDBkMjkwYWQxNDYxOTJlMDkxZTI2NiJ9.1iBnDz1Ac_94s8gamLULyl4nFji03fxGNQUFKJqojmrXaNHCdFHUy37BuP4d4bkiQGkhvUxcUDQK7Dn-RxkR3g)

The repository consists of two folders: 
- Dataset: contains the primary dataset of article [] we used companion with additional data we fetched using GitHub rest API. 
  
- Features: contains sheets of data that represent different combinations of original dataset fields we created to facilitate score calculations.
  
In code files, we used files in the dataset and features directories content referring by their address. We assumed dataset and features folders are in the same folder as jupyter notebooks. Also, our codes make some new files in a new directory named results beside notebooks.
