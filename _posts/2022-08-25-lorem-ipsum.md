---
layout: post
title: Preserving Cultural Heritage with the Help of an Ojibwe Verb Conjugator
subtitle: Student Capstone Project
cover-img: /assets/img/culturefoundry.jpg
thumbnail-img: /assets/img/culturefoundry-thumb.png
share-img: /assets/img/culturefoundry-thumb.png
---

Language is not only an important form of communication, but also important for the preservation of cultural heritage. This is particularly true of Indigenous languages.

[CultureFoundry](https://www.culturefoundrystudios.com/) is a remote-first, Canadian, social purpose ed-tech company that offers creative solutions to support language revitalization efforts in partnership with community. Their primary product is a customizable language learning platform that takes learners from beginner concepts to basic fluency, using interactive and engaging elements that centre around oral traditions and first speaker-created lesson plans and modules. Working with community leaders and knowledge keepers, the platform can be adapted to any language. 

CultureFoundry was looking to improve/re-develop the conjugation tool within the platform for nouns and verbs within various Indigenous languages, such as Ojibwe. This tool allows language learners to smoothly and efficiently navigate the many possible forms each word can take, giving them greater authority and confidence in building their language skills. 

This is where CultureFoundry turned to a group of UBC Master of Data Science Computational Linguistics students, who created an Ojibwe conjugator and API (Application Programming Interface) to tackle this task.

The goal of the conjugator was to return suggestions for verbs to conjugate from their search (either in English or Objiwe), then to return the correct conjugation for the verb that was chosen.

The Ojibwe language is quite different to English, so the students needed to create a solution that understood the different ways that verbs change based on subject and object.

The students solved the verb conjugation problem by using a finite state transducer, which is a finite state machine with an input tape and an output tape. The input was the polarity, sentence form, tense, object tags and the verb stem itself. The output was the conjugated verb form.

The API developed by the group connected the Ojibwe conjugator website with the new database they created. The API had two functions: The suggestion function and the conjugation function.

The suggestion function returned a list of possible verbs from the database, based on what the user typed into the search bar. Once the user chose a verb from the list, it would be conjugated through the conjugation function.

The conjugation function also had several parameters, such as a Language Connection Parameter (LANG), which was either English or Ojibwe, as well as a dialect parameter, to choose which dialect of Ojibwe you wanted the verb conjugated into. To create the conjugation, the function required the verb stem and class, polarity, form, subject, object and tense. 

Through this project, the MDS Computational Linguistics students created a tool to aid in language revitalization that will be useful for Ojibwe language learners and teachers. The CultureFoundry team is hopeful that this tool can be used for other complex languages, and is looking forward to working with another group of UBC students in the future. 
