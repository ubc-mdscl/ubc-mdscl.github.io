---
layout: post
title: Revelo Magicen – The Harry Potter Spell Hunt
subtitle: Student Data Science Project
cover-img: /assets/img/harry-potter.jpg
thumbnail-img: /assets/img/harry-potter-thumb.png
share-img: /assets/img/harry-potter-thumb.png
---

When asked to create a novel annotated corpus that could be used by others for analysis or machine learning for their Advanced Corpus Linguistics class, a group of MDS Computational Linguistics students (Saffrin Granby, Mariia Shubina, Mrinal Grover, and Varadraj Ramesh Poojary) focused on investigating the specific emotion in Goodreads book reviews.

The reviews on Goodreads range from short to long, negative to positive describing a user’s reading experience. This led the students wanting to investigate the specific emotion of these book reviews, compare the emotion to the ratings and also how emotions could differ across different book genres.

To build their dataset for emotion detection and classification, the group used a library called BeautifulSoup along with a tool called Selenium to parse the HTML of a book page and extract a book’s title, author, genre, and 10-20 reviews from the book as well as the writer’s rating. 

Knowing that emotion labeling can be a very subjective task, the students used Mechanical Turk to annotate their data on a small set of their data, which consisted of 465 reviews. The turkers were asked to read a review and then classify a review into one of the following emotions: enthusiastic, sad, bored, disappointed, content, love, neutral. 

![Harry Potter Spell Dashboard](https://ubc-mdscl.github.io/assets/img/harry-potter-img.png)

While some of the turkers annotated the groups’ small dataset correctly, not every turker completed the task properly. Even when considering that emotion classification is subjective, there were many cases where a review would be clearly very positive and the turker would have labeled it as bored or disappointed. To overcome this hurdle, the students used only a subset of the reviews with a higher inter-annotator agreement in their final annotated corpus. The most common emotion noted across the 465 reviews was enthusiasm, which was 27% of the total.

The students then created a website that shows the user the group’s corpus and allows them to search through it by book title, author, genre, rating, and emotion. 

The students hope that the results of their project can be used by other people to train their models to recognize certain emotions in the context of reviews.

As fans of the Harry Potter book series, four MDS Computational Linguistics students (Xinyi Li, Boyang Liu, Zimo Wang, and Yiting Zhou) from the Class of 2022 knew they wanted to annotate spells from the books for their Advanced Corpus Linguistics project.

The project tasked students to collect a large corpus from the web, carry out reliable corpus annotation using external annotators and make the corpus searchable via HTML frontend and Python backend.

In addition to annotating all the spells from the books, the group decided to track all the spells in terms of when they are used, in which cases are they used, who are using them and come up with some analysis of them.

To start, the students found a website that had all the e-book versions of the Harry Potter books. Their data set comprised 1,084,170 words of raw text, which they extracted around 730 annotations.

The students wrote a Python script that found paragraphs that contain mentions of spells. 

While working on the annotation of their data corpus, the students found that it could be ambiguous or confusing to make certain annotation and it could be biased potentially, so they came up with a protocol, namely “Interannotator agreement”, which involved splitting up the annotation task to each member. With work overlapping between two annotators, they were able to evaluate the accuracy score of annotation and eliminate some misleading information.

From their findings, the group discovered that Harry is the person who casts the most spells and also receives the most spells. As well, there’s a lot of day-to-day magic in the book rather than just killing or attacking spells. 

The end result was implementing a web app using simple Python and HTML scripts and wrapped it in Docker for it to be visualized properly. To make the app work, a user would download the required Docker file and open it locally, then follow the instructions provided.

The students hope that this type of annotation would inspire fans of other books to do similar work and that by combining programming and manual annotation, fans can dig a lot deeper into the characters and scenarios of any book.
