---
layout: post
title: BookdelTest - Female Participation in Jane Austen Novels
subtitle: Student Data Science Project
cover-img: /assets/img/path.jpg
thumbnail-img: /assets/img/thumb.png
share-img: /assets/img/path.jpg
---

The Bechdel Test was created by cartoonist Alison Bechdel as a tool used to evaluate the representation of women in media. The work passes this test if it includes a scene where at least two main female characters have a conversation about something other than a man. 

For their Advanced Corpus Linguistics project, a group of MDS Computational Linguistics students (Ananya Apparaju, Michelle Yun, Sara Mirjalili, Jata MacCabe, and Kai Maurin-Jones) wanted to adapt this test to assess female participation in Jane Austen's novels. Jane Austen was a celebrated 18th century English author known for her examination of marriage and the role of women in society.

In the group’s “Bookdel” test, the aim of the project was to uncover how Austen’s works portray female characters in relation to their societal expectations.

While there are plenty of websites dedicated to applying the Bechdel Test to movies and TV shows, there really isn’t an equivalent for novels. Novels lack a defined structure without explicit labels for scene boundaries, speakers and dialogue. It's much harder to say what a scene entails or where a conversation ends. 

In order to keep their annotation consistent, the group decided to make a chapter analogous to a scene. However, the group still found that co-reference resolution and character identification remained a challenge. For example, in the novel “Pride and Prejudice”, Miss Bennett can refer to five different characters.

The group applied automated approaches such as Stanford's Named Entity Recognizer but found it performed poorly on their corpus. Eventually, the students decided to manually create a dictionary mapping each character and their gender to every possible alias for co-reference. Pronouns were co-indexed with the nearest preceding character, with the same gender.

To create annotations, the students looked for all dialogue within a chapter. Once identified, they split the relevant paragraph into text inside and outside the dialogue. Within dialogue, characters were tagged as mentions and outside dialogue, characters were tagged as speakers. 

The group developed a web app where users can search whether Jane Austen’s books passed the Bechdel Test. The app also lets people filter to see all male speakers and all female speakers in an entire book. The app also lets people filter specific chapters in a book. 

![Screenshot of the group's web app](https://ubc-mdscl.github.io/assets/img/final-bookdel-img.png)

Of all the 238 chapters in the books the group analyzed, only one chapter actually passed the Bechdel Test (chapter 23 of “Sense and Sensibility”). The group summarized that Jane Austen’s books shouldn’t be called sexist but is just an indication of how integral men were to the story in relation to the female characters and their experiences were often still defined by or in relation to the male characters around them.

The students think that their corpus could be a valuable resource for readers who want to revisit Jane Austen's works with a focus on modern feminist ideas.
