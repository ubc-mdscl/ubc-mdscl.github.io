---
layout: post
title: Cross-Lingual NER for Low-Resource Languages
subtitle: Student Capstone Project
cover-img: /assets/img/crossling.png
thumbnail-img: /assets/img/crossling-thumb.png
share-img: /assets/img/crossling-thumb.png
---

For their capstone project, a group of UBC MDS Computational Linguistics students were tasked by Seasalt.ai, a conversational AI start-up, to create a universal NER (Named Entity Recognition) system with fine-grained labels for multiple low-resource languages.

NER is an information extraction method that classifies named entities in a text into multiple categories (or labels), such as person names, locations, organizations, and datetimes.

Current models used to extract NERs, like spaCy models, only support 18 labels (i.e. ORG, GPE, NORP) and only high-resource languages, such as English, French, German and Chinese. This is not practical for industry use as more granularity is needed and countless low-resource languages, including Indonesian, Javanese, Malay, Vietnamese, Tagalog, Croatian, and Czech, are not represented. 

One of the biggest challenges for students was that there was no available data with fine-grained labels to train a low-resource language NER model. Therefore, the team decided to leverage the existing system and its high-resource language datasets to apply transfer learning onto low-resource languages. The team worked with data that included 300K untagged raw sentences from Wikipedia Simple English Dump and 140K English and 40K Chinese sentences with 18 labels from Ontonotes (a large corpus comprising various genres of text), and used DBpedia Ontology to tag organizational companies.

The MDS-CL students used a model, called XLM-RoBERTa, that was pretrained on 100 languages, including Indonesian, Javanese, and Croatian. Because it was a multilingual model, it was able to learn NER knowledge from high-resource languages and apply it to low-resource languages.

The system developed by the team managed to extract 34 fine-grained labels (i.e. city, country, nationality) from the example English sentences and also worked on close to 10 low-resource languages.
Looking at the data, the students discovered that the low-resource Asian languages outperformed the European low-resource languages by quite a margin. For example, Javanese had an f1-score of 80.87% versus Croatian at 49.86%. The average f1-score achieved for the team’s model was 64.33% on eight human annotated data.

NER data can be applied in various NLP tasks, including chatbots, text summarization, and smart speakers, which is why expanding on the number of languages included is so extremely important.
