---
layout: post
title: Phase One of a Universal Graded Reader
subtitle: Student Capstone Project
cover-img: /assets/img/graded-reader.jpg
thumbnail-img: /assets/img/graded-reader-thumb.png
share-img: /assets/img/graded-reader-thumb.png
---

Graded readers are levelled reading materials that help language learners improve, by detecting stories and other media that are just slightly above the learner’s current level in the language.

While there is great demand for graded readers across all languages, the creation of graded readers is manual and time-consuming, especially if there is not enough data, which is the case for many languages.

Could computational linguistics provide a better, faster solution?

That was the question posed by faculty members at UBC Linguistics and UBC French, Hispanic, and Italian Studies departments to a group of MDS Computational Linguistics students for their capstone project.

The standard for assigning levels to text is the Common European Framework of Reference for Languages (CEFR). CEFR assigns six levels for grading a text, ranging from A1/A2 (beginner) to B1/B2 (intermediate) and C1/C2 (native). For this particular project, the MDS-CL students worked with the Spanish language only and limited their scope to A1, A2, and B level documents to focus on the functionality required for beginner language learners.

The data that the MDS-CL students used included Spanish texts from a variety of sources, such as “An Elementary Spanish Reader,” “Aventura Joven,” and “Spanish Tales for Beginners.” The text styles ranged from poems to short stories to news articles.

The first phase of the project involved developing a machine learning system that could automatically assign a reading level to any text it was given.

The students tried several approaches to classifying reading levels for the scraped text, including a simple rule-based model, complex tree-based models, and a Support Vectore Machine (SVM) Classifier. Whereas the team found that these statistical models performed relatively well, as they had hoped, the students implemented a state-of-the-art neural model, which ended up outperforming the rest. 

To train the models, the group developed various linguistics features to capture the characteristics of each text, such as A-level vocabulary (percentage of words in the text that are A-level words) and syllables per sentence (the average number of syllables per sentence). The team used these features to improve the machine learning algorithm and help classify the text.

