# Detecting - Humor & Offense

## **Introduction:**

- Humor, like most figurative language, poses interesting linguistic challenges to NLP, due to its emphasis on multiple word senses, cultural knowledge, and pragmatic competence. Humor is an essential but most fascinating element in personal communication.
- In this project, we worked on a dataset with labels and ratings from a balanced set of age groups from 18-70.
- We have created two Model which is used to predict whether the text is humorous, if it is humorous, what is the humor rating and humor controversy whereas if the text is offensive, how offensive it is.

## **Relevant Domain Information:**
 https://competitions.codalab.org/competitions/27446

##  **Data understanding :**
CodaLab has provided training and test datasets in Train.csv and Test.csv respectively. 
### Train.csv: 
This is the training dataset with 8000 records. In this data, we had 6 columns: **ID**, **Text**, **is_humor**, **humor_rating**, **humor_controversy**, **offense_rating**

### Test.csv: 
This is the training dataset with 1000 records. In this data, we had 2 columns: **ID**, **Text**

## EDA:

![1](https://github.com/Anisha-Kakwani/Hahackathon---Detecting-Rating-Humor-Offense/blob/master/Images/Picture1.png?raw=true)


![2](https://github.com/Anisha-Kakwani/Hahackathon---Detecting-Rating-Humor-Offense/blob/master/Images/Picture2.png?raw=true)


![3](https://github.com/Anisha-Kakwani/Hahackathon---Detecting-Rating-Humor-Offense/blob/master/Images/Picture3.png?raw=true)


![4](https://github.com/Anisha-Kakwani/Hahackathon---Detecting-Rating-Humor-Offense/blob/master/Images/Picture4.png?raw=true)


##  **Machine Learning :**

- For detecting Sarcasm on the given dataset, we started by creating model using **Linear SVC** approach and **Naive Bayes**.
- Linear SVC model gave accuracy of **58.3%** and Naive Bayes model gave accuracy of **79.3%**.
- Later on we decided to start  experimenting with TensorFlow model and we tried various model like **ColBERT**, **LSTM**, **wordEmbedding** with 4 layer model and one **without wordEmbedding** , and **GRU** . 
- Among all this ColBERT gave the highest accuracy of **91.5%** in predicting if text is humor or not.
- GRU gave **63.7%** accuracy, LSTM provided accuracy of **76%** and NN model with Word Embedding gave accuracy of **83.5%** .


## **Future Work**:

Here as we see accuracy of **83.5%** in neural network model, we can work more on that model (boost the model) and also we can fine tune ColBERT model and try to get more accuracy.

## Reference:

- https://arxiv.org/pdf/2004.12765.pdf
- https://github.com/manashpratim/Sarcasm-Detection/blob/master
- https://www.youtube.com/watch?v=-8XmD2zsFBI

