<img src='https://www.salesforce.org/wp-content/uploads/2021/02/uva-university-of-virginia-logo.png' width=300 align='center'/>

# Machine Learning with Coronavirus Data

## Description
Completed during a four-week Independent Study taken through the Computer Science department at the University of Virginia; worked as a research assitant for [Professor Haiying Shen](https://engineering.virginia.edu/faculty/haiying-shen).

Project aims to test the performance of various Machine and Deep Learning algorithms in predicting the result of a Coronavirus-19 test. The entirety of the project was completed in Python, using Jupyter Notebooks. In total, six algorithms were tested, three from [scikit-learn](https://scikit-learn.org/stable/index.html) and the other three from [Keras](https://keras.io/); proper citations for these libraries are listed below. The final list of algoritms is as follows:
* Decision Tree Classifier
* Random Forest Classifier
* K-Nearest Neighbors Classifier
* Deep Neural Network
* Convolutional Neural Network
* Recurrent Neural Netowrk

A final report detailing model performance and research procedure was completed, but it is not included in the repository.

## Table of Contents
#### Files
Number | Filename | Last Update
------------ | ------------- | -------------
1 | [ml_covid_research](https://github.com/iainmuir6/Machine-Learning-with-Coronavirus-Data/blob/master/ml_covid_research.ipynb) | June 8th, 2021
2 | [ml_covid_research_w2](https://github.com/iainmuir6/Machine-Learning-with-Coronavirus-Data/blob/master/ml_covid_research_w2.ipynb) | June 15th, 2021
3 | [ml_covid_research_w3](https://github.com/iainmuir6/Machine-Learning-with-Coronavirus-Data/blob/master/ml_covid_research_w3.ipynb) | June 21th, 2021
4 | [ml_covid_research_final](https://github.com/iainmuir6/Machine-Learning-with-Coronavirus-Data/blob/master/ml_covid_research_final.ipynb) | July 9th, 2021

#### Final Script Table of Contents
* **[0. Import Packages](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#setup)**
    * [0.1 General Imports](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#imp1)
    * [0.2 ML Imports](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#imp2)
* **[1. Read Excel File](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#data)**
    * [1.1 Data Overview](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#overview)
    * [1.2 Descriptive Statistics](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#stats)
    * [1.3 Inspect Null Data](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#null)
* **[2. Data Preparation](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#prep)**
    * [2.1 Drop Columns](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#drop)
    * [2.2 Handle Categorical Variables](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#handle1)
        * *[2.2.1 Manual Conversion](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#manual)*
        * *[2.2.2 Encoding](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#encoding)*
        * *[2.2.3 Categorical Codes](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#codes)*
    * [2.3 Handle Missing Values](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#handle2)
    * [2.4 Feature Scaling](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#scaling)
    * [2.5 Train / Test Split](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#split)
    * [2.6 Final Prepared Data](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#final_data)
* **[3. Feature Selection I](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#feature)**
    * [3.1 Pearson Correlation](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#corr)
    * [3.2 Chi-Squared Test](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#chi_sq)
    * [3.3 Recursive Feature Elimination](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#rfe)
    * [3.4 SelectFromModel: Lasso](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#lasso)
    * [3.5 SelectFromModel: Random Forest Classifier](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#rfc)
    * [3.6 Cumulative Feature Selection](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#cum)
* **[4. Model Selection](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#model)**
    * [4.1 Train / Test Data](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#tt)
    * [4.2 Model Evaluation Functions](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#funcs)
    * [4.3 Model Construction](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#models)
        * *[4.3.1 Decision Tree](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#dt)*
        * *[4.3.2 Random Forest Classifier](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#rfc2)*
        * *[4.3.3 K-Nearest Neighbors Classifier](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#knn)*
        * *[4.3.4 Deep Neural Network](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#dnn)*
        * *[4.3.5 Convolutional Neural Network](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#cnn)*
        * *[4.3.6 Recurrent Neural Network](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#rnn)*
    * [4.4 Simultaneous Model Evaluation](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#eval)
    * [4.5 RandomizedSearch](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#search)
* **[5. Generative Adverserial Networks](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#gan)**
    * [5.1 Network Setup](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#setup2)
    * [5.2 Training GAN Models](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#train)
        * [5.2.1 GAN](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#gan2)
        * [5.2.2 CGAN](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#cgan)
        * [5.2.3 WGAN + WCGAN](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#wgan)
    * [5.3 Loss Information](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#loss)
    * [5.4 Generate New Data](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#new_data)
    * [5.5 Training Models on New Data](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#train_gan)
    * [5.6 Plot Real vs Test Data](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#plot)
    * [5.7 Feature Importance](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#importance)
* **[6. Retrain Models with GAN Data](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#retrain)**
    * [6.1 Re-Prepare Data](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#prep2)
    * [6.2 Re-Train Models](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#retrain2)
* **[7. Final Model Training with Feature Selection](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#final)**
    * [7.1 Define Models and Variables](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#define)
    * [7.2 Model Performance w/o GAN](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#perf1)
    * [7.3 Model Performance with GAN](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#perf2)
* **[8. Figures for Final Report](http://localhost:8888/notebooks/ml_covid_research_final.ipynb#figures)**

## Credits
[scikit-learn](https://scikit-learn.org/stable/index.html)
```
@article{scikit-learn,
 title={Scikit-learn: Machine Learning in {P}ython},
 author={Pedregosa, F. and Varoquaux, G. and Gramfort, A. and Michel, V.
         and Thirion, B. and Grisel, O. and Blondel, M. and Prettenhofer, P.
         and Weiss, R. and Dubourg, V. and Vanderplas, J. and Passos, A. and
         Cournapeau, D. and Brucher, M. and Perrot, M. and Duchesnay, E.},
 journal={Journal of Machine Learning Research},
 volume={12},
 pages={2825--2830},
 year={2011}
}
```
[Keras](https://keras.io/)
```
@misc{chollet2015keras,
  title={Keras},
  author={Chollet, Fran\c{c}ois and others},
  year={2015},
  howpublished={\url{https://keras.io}},
}
```
