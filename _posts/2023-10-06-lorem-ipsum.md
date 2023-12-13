---
layout: post
title: Improving BC Data Catalogue with NLP Techniques
subtitle: Student Capstone Project
cover-img: /assets/img/bc-stats-image.png
thumbnail-img: /assets/img/bc-stats-image.png
share-img: /assets/img/bc-stats-image.png
---

The BC Data Catalogue contains over 3,000 government datasets with lots of useful information, available for anyone to use. Despite its wealth of information, users often faced difficulties in locating the datasets they needed, resulting in lower engagement with the platform. Recognizing this challenge, BC Data Service identified two key barriers hindering user satisfaction. 

The first barrier was a suboptimal search quality, where users struggled to find the desired datasets unless they used exact keywords. Second, there was no clear overview of the datasets, making it hard to know what topics the datasets covered and how many datasets there were for each topic.  

To address these challenges and enhance the user experience, BC Data Service sought the expertise of a group of MDS Computational Linguistics students. 

To tackle the search issue, the team leveraged Semantic Search, an advanced NLP technique focused on understanding user intent rather than relying solely on specific keywords. The team used Bert to implement semantic search on top of catalogue’s search engine, leading to a substantial improvement in search performance. The new search engine has the ability to comprehend synonyms and phrases. It can also handle typing errors, making it more intuitive and user-friendly.  

Additionally, to provide a comprehensive grasp of the datasets, the team employed Topic Modeling, an unsupervised machine learning technique, using transformers and c-TF-IDF. Through topic modeling, the datasets were categorized into distinct clusters based on their similarities. Each category was then associated with several descriptive labels. To present this insightful categorization, the team employed three different types of interactive visualizations, allowing users to gain a clearer understanding of the dataset landscape. 
