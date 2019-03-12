# Capstone: Philosophical Factors for NLP
**_Identifying Similarity to Philosophical Worldviews in Text Data_**

## Thomas W. Ludlow, Jr.
**General Assembly Data Science Immersive DSI-NY-6**

**February 12, 2019**

## Problem Statement

**How well can Machine Learning models recognize the ideas of historic philosophers?**  
**Goal: Build a Natural Language Processing (NLP) model that identifies the philosophical factors for any text input using predictive similarity.**

## Executive Summary

This Capstone Project for General Assembly's Data Science Immersive program is a Multiclass Classification Natural Language Processing model, set to compare text to models trained on a corpus of historic philosophical texts.  The model uses features designed with Gensim to extract semantic meaning from the text: Latent Dirichlet Allocation (LDA) and Document Vectorization (Doc2Vec).  These features are processed using 3 models: Logistic Regression, Multinomial Naive Bayes, and Front-Feeding Recurrent Neural Network.  

The following sections are supported by the respective numbered Jupyter Notebooks.

#### 1. EDA and Preprocessing


#### 2. LDA Topic Modeling


#### 3. Document Vectors


#### 4. Multiclass Classifier Models


#### 5. Factorizing Unseen Text



## Data Dictionary

**Text Metadata**

|Feature|Type|Dataset|Description|
|---|---|---|---|
|**Title**|*object*|Train/Test|Title of philosophic work|
|**Author**|*object*|Train/Test|Author name|
|**Filename**|*object*|Train/Test|Target filename|
|**Start Key**|*object*|Train/Test|First line to include from text|
|**End Key**|*object*|Train/Test|Last line to include from text|
|**Category**|*object*|Train|Type of philosophy|
|**Bumper Sticker**|*object*|Train|Sentence summary of philosopher's attributed view|
|**Original Language**|*object*|Train|Original language of publication/recording|
|**Country**|*object*|Train|Original country of publication/recording|
|**Year**|*object*|Train|Year of publication, incl BC, ~ for approximation|
|**Year Val**|*int*|Train|Year of publication numeric, with BC as negative|
|**Wiki Link**|*object*|Train|URL for Wikipedia reference|
|**Wiki Text**|*object*|Train|Text from Wikipedia reference|
|**Paragraphs**|*int*|Train/Test (after preprocessing)|Count of paragraphs in work|

**Preprocessed Corpora**

|Feature|Type|Dataset|Description|
|---|---|---|---|
|**author**|*object*|Train/Test|Author|
|**work**|*object*|Train/Test|Title of philosophic work|
|**a_num**|*int*|Train/Test|Author number, shared for multiple works|
|**w_num**|*int*|Train/Test|Work number, unique|
|**p_num**|*int*|Train/Test|Paragraph number in work|
|**s_num**|*int*|Train/Test|Sentence number in paragraph|
|**sent_text**|*object*|Train/Test|Original printable sentence text with punctuation|
|**sent_lemma**|*object*|Train/Test|Preprocessed sentence lemma as list|
|**par_text**|*obj*|Train/Test|Original printable paragraph text with punctuation|
|**par_lemma**|*obj*|Train/Test|Preprocessed paragraph lemma as list|

**LDA and Doc2Vec Corpora**

|Feature|Type|Dataset|Description|
|---|---|---|---|
|**p_num**|*object*|Train/Test|Paragraph number in work|
|**s_num**|*object*|Train/Test|Sentence number in paragraph|
|**lda_s_\[0-31]**|*float*|Train/Test|Vectors for LDA sentence 0-31|
|**lda_p_\[0-19]**|*float*|Train/Test|Vectors for LDA paragraph 0-19|
|**d2v_s_\[0-31]**|*float*|Train/Test|Doc2Vec for sentence 0-31|
|**d2v_p_\[0-15]**|*float*|Train/Test|Doc2Vec for paragraph 0-15|
|**a_num_\[one hot encode]**|*int*|Train/Test|Author number (Target value)|


## Conclusions & Recommendations




#### Recommendations



## Data Sources

Project Gutenberg: www.gutenberg.org
ETEXT: www.textfiles.com/etext