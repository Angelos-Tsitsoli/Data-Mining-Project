<img src="https://github.com/user-attachments/assets/a6908861-0da1-4708-9eb9-5efade28f390" alt="Airbnb_Logo_Bélo svg" width="200"/>

# Assignment #1

## Preview 
In this project, you will work with data from a well-known home rental application (airbnb). Specifically, you are given the data for the Athens area for 3 months in 2019 and 2023. The data is in CSV format, and you will use Python to answer the some questions.

## Description
- Data exploration (using the following to answer the questions of the first part of the project):
  - Data cleaning
  - Missing data handling
  - Creation of heatmap,histograms
  - Use of library Folium Map
- Reccomendation System 
  - Creation of the TF-IDF matrix for the unigrams and bigrams using the parameter stop_word of TfidfVectorizer.
  - Use of Cosine Similarity for the calculation of the similary between the vectors.
  - Prediction for the most similar vectors in each case.
  - Use of BigramCollocationFinder to find words that appear frequently together.


# Assignment #2
# Study over time  
- Use of HuggingFace for the annotation process: Sentiment (positive/negative/neutral) should be annotated for as many comments as possible from 2019. The dataset can be split into smaller chunks, allowing the annotation to be performed in segments. The final output should include an identifying ID, resulting in a CSV file (or dataframe) with 3 columns: id, review, and sentiment.
- The same process should be applied to the reviews from 2023.
- A comparison of the overall sentiment over time should be conducted (e.g., by creating a histogram for each year, showing the distribution of positive/negative/neutral sentiments).
- Sentiment should also be compared by neighborhood over time .

# Sentiment Analysis
- Creation of two datasets (train.tsv,test.tsv)
- Setting the characteristics for every review using:
  - Tf-idf
  - Word embeddings
- Using the pickle Python store the characteristics in .pkl files.
- Use the following classifiers for the training:
  - SVM
  - Random Forests
  - KNN
-For the evaluation of the classifiers performance use 10-fold Cross Validation with these parameters:
  - Precision/Recall/F-Measure
  - Accuracy

# Similarity (jaccard, cosine, etc) and semantic neighborhoods
- For the comments column and using word embeddings, create a function that will calculate the similarity between the vectors of two words (e.g., cosine or any other method you prefer). Us any method that creates word embeddings like word2vec. fastText, glove.
- For a set of words find:
  - Τhe semantic neighborhood of the words.
  - the similarity of the words which will result from the neighborhood based on the three figures below, i.e. 3 different similarities
  

<img src="https://github.com/user-attachments/assets/d4a3b31f-5830-4515-a618-5726e9ef2c1c" alt="Image svg" width="200"/>
