# RCC-Finder
This repository contains all source codes of RCC-Finder, a heuristc code reviewer recommender system. codes folder consists of 7 jupyter notebook. We try to chose each notebook name in a way help to understand its function. here is  brief explanation of source code files:
  
  1) WhDo reimplementation: contains reinplementation of WhoDo, the recommender system with which we compare our proposed approach.
  
  2) preparetion: contains code of some primary data modifications, such as selecting pull requests which has been reviewed and finding all candidate reviewers.
  
  3) relative scores calculation: Basic commit and review scores are obtained in WhoDo reimplementation. In this file we caculate relative commit and review scores based on 
  those   basic ones. 
  
  4) former packs change score: WhoDo consider commit experience on files and last level directories. In this file we try to test commit score for direcories in the level 
  preceding the last level.
  
  5) review and commit scores calculation with different time coefficients: RCC-finder consider recency of commit and review experiences. This file contains source code for   
  calculating scores using different time coefficients. 
  
  6) calculate collaboration score: contains source code for calculating collaboration score.
  
  7) calculate activity score using 5 different methods: contains of five different methods we tried to calculate activity score through
  
Our dataset is accessibe through Zenodo link bellow:

The repository consists of two folders: 

  1) dataset which contains the primary dataset of article [] we used companion with additional data we fetched using GitHub rest API. 
  
  2) features: contains sheets of data represents different combinations of original dataset we created to facilitate scores calculations.
  
In code files we read dataset and features files content refering by address. We assume which dataset and features folders are in the same folder as jupyter notebooks. Also, our codes make some new files in a new directory beside notebooks named results.
