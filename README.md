# bert_cord19
Passage retrieval on CORD-19 dataset with different pretrained BERT models

## Platform
Google Collab

## Language
Python

## Libraries
PyTorch, Transformers, Pandas, Numpy, Skipy

## Description / Goals 
The purpose of this project is the developement of a document retrieval system that returns titles and passages of scientic papers containing the answer to a given user question. In order, to achieve that we use different pretrained BERT models applied on the latest version of the COVID-19 Open Research Dataset (CORD-19). Specifically, we process the articles in the folder 'comm_use_subset' and we utilize the metadata provided in the 'all_sources_metadata_2020-03-13.csv' file. <br>
We implement 2 models for the titles retrieval task and 2 different models for the passages retrieval task. We evaluate our experiments based on the mathematical-theoretical background of each model. We compare the results of our models based on:
* their architecture
* their execution time
* the cosine similarity score of the retrieved answer

## Examples
1. **Question:** What are the coronaviruses? <br>

**Title:** Infectious Bronchitis Virus Nonstructural Protein 4 Alone Induces Membrane Pairing <br>
**Score:** 8.640386581420898 <br>
**Abstract:** **positive-strand rna viruses**, such as coronaviruses, induce cellular membrane rearrangements during replication to form replication organelles allowing for efficient viral RNA synthesis. <br>

2. **Question:** What is caused by SARS-COV2? <br>

**Title:** The Disulfide Bonds in Glycoprotein E2 of Hepatitis C Virus Reveal the Tertiary Organization of the Molecule <br>
**Score:** 7.8293867111206055 <br>
**Abstract:** Hepatitis C virus (HCV), a major cause of **chronic liver disease** in humans, is the focus of intense research efforts worldwide. <br>

3. **Question:** what are the public measures to control the spread of covid-19? <br>

**Title:** Local risk perception enhances epidemic control <br>
**Score:** 7.057101249694824 <br>
**Abstract:** As infectious disease outbreaks emerge, public health agencies often enact **vaccination and social distancing measures** to slow transmission. <br>

## Tips
Add the 'comm_use_subset' directory and the 'all_sources_metadata_2020-03-13.csv' dataset in your 'gdrive/My Drive/Colab Notebooks/' path to execute correctly

Suggested Runtime Type: GPU

## Author
Vassilis Panagakis

## Date
February 2021
