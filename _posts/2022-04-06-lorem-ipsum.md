---
layout: post
title: Detecting Emotion in Goodreads Book Reviews
subtitle: Student Data Science Project
cover-img: /assets/img/goodreads.png
thumbnail-img: /assets/img/goodreads-thumb.png
share-img: /assets/img/goodreads-thumb.png
---

When asked to create a novel annotated corpus that could be used by others for analysis or machine learning for their Advanced Corpus Linguistics class, a group of MDS Computational Linguistics students (Saffrin Granby, Mariia Shubina, Mrinal Grover, and Varadraj Ramesh Poojary) focused on investigating the specific emotion in Goodreads book reviews.

The reviews on Goodreads range from short to long, negative to positive describing a user’s reading experience. This led the students wanting to investigate the specific emotion of these book reviews, compare the emotion to the ratings and also how emotions could differ across different book genres.

To build their dataset for emotion detection and classification, the group used a library called BeautifulSoup along with a tool called Selenium to parse the HTML of a book page and extract a book’s title, author, genre, and 10-20 reviews from the book as well as the writer’s rating. 

Knowing that emotion labeling can be a very subjective task, the students used Mechanical Turk to annotate their data on a small set of their data, which consisted of 465 reviews. The turkers were asked to read a review and then classify a review into one of the following emotions: enthusiastic, sad, bored, disappointed, content, love, neutral. 

![Goodreads Dashboard](https://ubc-mdscl.github.io/assets/img/goodreads-img.png)

While some of the turkers annotated the groups’ small dataset correctly, not every turker completed the task properly. Even when considering that emotion classification is subjective, there were many cases where a review would be clearly very positive and the turker would have labeled it as bored or disappointed. To overcome this hurdle, the students used only a subset of the reviews with a higher inter-annotator agreement in their final annotated corpus. The most common emotion noted across the 465 reviews was enthusiasm, which was 27% of the total.

The students then created a website that shows the user the group’s corpus and allows them to search through it by book title, author, genre, rating, and emotion. 

The students hope that the results of their project can be used by other people to train their models to recognize certain emotions in the context of reviews.
