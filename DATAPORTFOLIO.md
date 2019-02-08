
---

### Data Science Portfolio

---

#### Exploratory Data Analysis
Mostly work from graduate level courses CISC873 Data Mining (Fall 2018) and CISC867 Deep Learning (Winter 2019).
In CISC873, I was assigned support vector machines and stacked denoising autoencoders to work with for the entire semester.

- Telecom Company Churn Predictions 📞
  - dataset already clean
  - data comes from IBM and can be found on [kaggle](https://www.kaggle.com/blastchar/telco-customer-churn/kernels)
  - classification
  - [Jupyter notebook](https://github.com/leblanchannah/DataMining873/blob/master/873groupAset1churn/churn.ipynb)
  - results: Based on visualizations, issues with fibre optic services and month-to-month contracts seem to make customers leave the telecom company. When focusing on customers who have been with the company for more than 12 months, it becomes extremely difficult to predict which customers will churn. Using SVM with a linear kernel, feature importance values indicate that paperless billing is important for predicting which customers will stay. Features total charges, extra fees and tenure are important for predicting which customers will leave. Recursive feature elimination shows that reducing the dataset to 14 features including the first principal component achieves similar results to the full dataset with SVM. The use of SMOTE does not seem to help prediction performance even though the original dataset is imbalanced. 
  
  
  
- California Crime Rates 👮‍♀️
  - messy and lots of missing data
  - given this dataset by prof
  - regression but as a class decided to make it classification
  - [GitHub Repo](https://github.com/leblanchannah/DataMining873/tree/master/873groupAset2crime)
  - results: Overlap between the robbery, property, burglary, larceny and motor vehicle theft classes makes this regression problem especially difficult. After one week of working on this dataset, the class as a whole decided to group together crime rates into classes. Along with classes overlapping and being a multilabel problem, there is a lot of missing data making this dataset very difficult to work with. Many counties within California are missing data for the majority of their columns making it difficult to impute data. Also, rows are labeled with year 1 or 2 without information on whether these two years are consecuitve. Features within the income and benefits category seem to contribute the most to crime rates. Counties with higher average number of people living within a household and low vacancies have lower crime rates. Having data on the amount of crimes that are actually solved/ cases closed would also be intersting. 
  
  
  
- Fraud Detection 🕵️‍♂️
  - imbalanced classes with a lot of missing data (missing values ends up being important)
  - dataset from
Dechow, Patricia M. and Ge, Weili and Larson, Chad Russell and Sloan, Richard G.,[Predicting Material Accounting Misstatements](https://www.thecaq.org/sites/default/files/DECHOW_et_al-2011-Contemporary_Accounting_Research.pdf) (April 21, Paper.2010). Contemporary Accounting Research, Forthcoming; AAA 2008 Financial Accounting and Reporting Section (FARS) 
  - classification
  - [GitHub Repo](https://github.com/leblanchannah/Fraud-Detection-SdA)
  - results: Unlike the above datasets, the fraud detection dataset uses features that are unclear to people like myself who are unfamiliar with accounting. The feature names makes it difficult to use real world experiences to interpret the graphs generated from this dataset as information is abstracted. There is also a lot of data missing in this dataset which ends up being useful, it seems like fraudulent companies attempt to obscure information or fail to give information. The addition of features that indicate which features are missing for a given company are helpful in this situation. For this dataset I was given the task to cluster the data using a stacked denoising autoencoder that I implemented with Keras. I compressed the data into a three dimensional and two dimensional latent layers and graphed the results. Although the graphs did not show the results I was expecting I think that more can be done to the autoencoder architecture to effectively learn latent features from the data. 


  
#### Natural Language Processing
- LCD Soundbook ⚡️
  - LCD Soundsystem lyric mining using Python, Genius API and Keras LSTM to generate lyrics 
  - first iteration [Jupyter notebook](https://github.com/leblanchannah/leblanchannah.github.io/blob/master/lcdsoundbook.ipynb)
  - results: The data from the Genius website is repetitive and user generated. The lyrics are generally trustworthy since multiple people can contribute and give feedback to user posted lyrics. I think more data is required to use an LSTM to generate lyrics since the lyrics come out repetitive. On the other hand, LCD Soundsystem's lyrics are very repetitve and I learned that it is difficult to gauge how well this approach does unlike my other projects that have clear cut metrics to evaluate performance. In the future, I want to experiement with algorithms that generate more structured lyrics rather than blobs of text and there is a plethora of other neural network models to try. 

 
 - Pitchfork Review Summarizer ([upcoming](https://github.com/leblanchannah/pitchfork-summary)) 🎸
    - So far I have used the Pitchfork Python API to download all album reviews and I have stored them in the repo. In the future I want to explore extractive summarization techniques with deep learning with the reviews. I also want to predict review score based on full review and generated summary features. 
    
#### Deep Learning
- Course assignment 1 
  - implementing a single hidden layer neural network using only NumPy and Python to learn the XOR function.
  - Outlines partial derivative for 2nd hidden layer.
  - Explores increasing weights to large numbers and saturation of sigmoid function.
  - [Jupyter notebook](https://github.com/leblanchannah/XOR-neural-network/blob/master/HannahLeBlanc.ipynb)
  




