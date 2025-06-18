---
layout: post
title: Ocarina Studios Dream Database
subtitle: Student Capstone Project
cover-img: /assets/img/dreamdatabase.png
thumbnail-img: /assets/img/dreamdatabase-thumb.png
share-img: /assets/img/dreamdatabase-thumb.png
---

Ocarina Studios is currently developing an adventure game as a tool for education. Ocarina’s Dream Database is a product that conceptually provides an infinite number of QA pairs from various topics to users, for both entertainment and educational purposes.

Ocarina’s Dream Database will be the main database system of Dream QuiZzz. In order for the database to grow, Ocarina worked with a group of UBC Master of Data Science (MDS) in Computational Linguistics students on a QA data retrieval project that will generate questions without the need for human work through the use of machine learning. Doing this will allow the knowledge base to grow at an exponential rate and to be used in a variety of sectors for entertainment and fun.

The students had access to a dataset with approximately 30,000 gold standard QA pairs along with their distractor answers and associated tags.  Furthermore, Ocarina provided the students with their database on AWS with raw scraped data based on different tags that are currently being used in the game. Finally, the students also had access to a simple web scraper, used to collect content on which the QA pairs are based.

The project was then divided into three main tasks: automating QA pair generation, tagging questions with relevant topics, and generating distractor answers.

The first step was to automate the creation of QA pairs. The group experimented with multiple different methodologies, involving Large Language Models (LLMs) and without, by using various traditional linguistic techniques.

For their next task, the students focused on ‘tagging’ the questions to associate them with specific topics or genres. They employed clustering methods and similarity scores to assign tags, such as “music” or “biology”.

The final task involved generating plausible yet incorrect answers (distractors) to make the trivia questions more challenging. The group fine-tuned an LLM model and explored pre-trained word embedding models. The students found this step particularly tricky as it required balancing the difficulty of the questions without making the distractors too obvious or too obscure.

Throughout the project, the students encountered several challenges. One of the main obstacles was dealing with unannotated data. The absence of annotated training data for some parts of the project spurred the students to come up with innovative methods for generating and validating question-answer pairs, ensuring the quality and relevance of their trivia content.

The group sees plenty of potential applications for this technology. From personalized learning platforms to interactive educational apps, the ability to generate tailored, summarized content on demand can transform how people learn and engage with information.

By integrating machine learning with web-crawled data, the students created a system that can continuously generate fresh and relevant trivia questions.

Parts of this article first appeared on [Medium](https://medium.com/@coloteong20/revolutionizing-the-gamification-of-knowledge-with-machine-learning-aeccaf5d786c) in a post written by the Ocarina capstone team.   
