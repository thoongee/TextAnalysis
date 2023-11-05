# TextAnalysis
2023-1 text analysis class

## 1. Overview
This is a team project for the Text Data Analytics class (← Is this English...? Check out the syllabus). E-commerce companies are attracting premium brands to increase customers, sales, and profitability. We planned this project to find answers to the following questions by comparing C.avenue products, a collection of premium brands from a leading Korean e-commerce company, with regular products.  
  - Do customers perceive premium brands selected by e-commerce companies differently from generic products?  
  - If customers perceive it differently, what makes it different from the norm?  

## 2. Project  
- Collecting data
  - coupang_crawling_0428.ipynb in Crawling folder
  - We targeted Coupang, a leading e-commerce company in Korea, and crawled product reviews on their site.  
  - We choose skincare reviews in the Beauty category and We crawled about 20,000 reviews.  
  - Limit to a minimum of 10 reviews per product to reduce bias  
  - Analyzed 1050 reviews each for C.Avenue and general products  
- PreProcessing
  - text_preprocess_tfidf.ipynb in preprocessing folder
  - Exclude special characters and emoticons for sentence-level analysis  
  - Exclude non-specific terms and trade names for stemming analysis  
  - Additional exclusions for investigative, indicative pronouns, etc.  
- TF-IDF & WordCloud
  - text_preprocess_tfidf.ipynb in preprocessing folder
  - WordCloud.ipynb in visualization folder
- Sentiment Analysis
  - sentiment_analysis.ipynb in sentiment_analysis folder (include training data)
  - Use a model trained on movie review sentiment analysis and CNN clssifier  
  - The review data was preprocessed on a sentence-by-sentence basis and the task was performed on 1050 reviews in each category.  
  - The result is a value between 0 and 1, where 0 is negative and 1 is positive.  
- Objective/Subjective Analysis
  - albert_small_model.ipynb in ObSub_analysis folder (include training data)
  - Use the pre-trained albert small model  
  - Training data: English objective/subjective data (used English data instead of Korean data, 5000 data each)  
  - We used the preprocessed data on a sentence-by-sentence basis and translated the preprocessed data into English before using it.  
  - The result is a value between 0 and 1, where 0 is objective and 1 is subjective.  
- Visualization
  - Graphs_visualization.ipynb in visualization folder
  - Display individual reviews in four quadrants  
  - Intuitively understand the differences between categories  
 
## 3. Conclusion
- Frequency analysis and positive/negative/objective/subjective analysis showed no difference between C.Avenue products and regular products.  
  - Consumers don't perceive C.Avenue products as different from regular products  
- Discover what makes a category different  
- Through this project, we were able to demonstrate how product reviews can be used for comparative analysis of product lines, and TF-IDF was able to reveal differences in characteristics that were not found through the usual frequency and sentiment analysis.
***
Utilize the following data file "merge_data.zip". This code was created with Colab.

If you have any questions, you can email here.  
dsekdls725@seoultech.ac.kr or cjina1102@seoultech.ac.kr 
