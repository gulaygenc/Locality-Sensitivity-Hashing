##### EN
# Detecting Plagiarism Between Documents using Locality Sensitive Hashing

**IDE Used:** Visual Studio Code

**Language Used:** Python

###### About:

This project was developed as part of my Master's Course Study in Algorithms and Methods for Big Data Analytics

The main motive of this project is to understand the process of how do we estimate the approximate or exact Near Neighbor Search in high dimensional spaces. The process flow includes 3 steps and they are:

1) Shingling: Obtains the k-shingles occurences between the documents.

2) Min Hashing: It involves 3 internal computation steps and they are: Generating Hash Function, Generating Signature Matrix and evaluating the fact check for obtained matrices using Jaccard Similarity with respect to the original wikipedia article.

3) Locality Sensitive Hashing (Candidate Generation): It takes the outputs scores obtained from Min Hahshing and performs the following steps:

--> Constructing Hash Signature Matrix based on the value of "L" into 'm' bands and 'n' rows.

--> Generating a Signature Vector for Original Wikipedia Articles and split them into 'm' bands and 'n' rows and hash them to same buckets of the original data which form the candidate documents.
    
--> Evaluting Jaccard Similarity between the candidate and original documents which completes the fact check.

--> Final step is to report the number of false positives and false negatives whose Jaccard Similarity Scores are compared to a value of "t".

###### Description about the files:

1) Project.pdf: This file contains the steps associated for developing the application and also the intermediate output formats for executing the program.

2) Locality_Sensitive_Hashing.py/Locality_Sensitive_Hashing.ipynb: Python program developed for detecting plagiarism between documents using Locality Sensitive Hashing and its associated internal steps.

3) corpus: Contains the input set of documents segregated into multiple "groups" of files for which I had processed and applied the steps involved in Locality Sensitive Hashing and detected the plagiarism between documents.

The given data corpus is made of short answers (200-300 words) to 5 basic Computer Science questions. The corpus contains 100 answers/documents - 95 documents (file names prefixed with ‘g’) represent answers given by 19 students for all 5 questions, and 5 documents (file names prefixed with ‘orig’) collected directly from Wikipedia articles.

4) corpus-final.xls: 
This corpus file defines various degrees of plagiarism. They are categorized into 4 types and they are:

    a) Cut: Answers were directly copied from the Wikipedia
  
    b) Light Revision: Copied with little alterations on words and phrases
  
    c) Heavy Revision: Each sentence is rephrased heavily into sentences with similar meaning
  
    d) Non-Plagiarism: Participants read Wikipedia articles and write answers based on their understanding
  
Output Files: The explanation about the output generated is available in "Locality_Sensitive_Hashing.ipynb" python file which explains clearly each step on how is the end result obtained.
  
##### TR


